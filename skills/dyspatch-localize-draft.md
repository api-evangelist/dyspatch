---
name: Localize a Dyspatch draft
description: >-
  Create and manage language variants of a Dyspatch draft — lock it for
  translation, list localization keys, set translations per language, and save or
  delete localizations. Use when producing a multi-language version of a message.
api: openapi/dyspatch-openapi-original.json
operations:
- lockDraftForTranslation
- getDraftLocalizationKeys
- getLocalizationForDraft
- saveLocalization
- getTranslations
- setTranslation
- deleteLocalization
- unlockDraftForTranslation
---

# Localize a Dyspatch draft

Produce language variants of a draft and manage their translations.

## Auth & conventions
- `Authorization: Bearer <DYSPATCH_API_KEY>` (read & write key).
- `Accept: application/vnd.dyspatch.2026.06+json`.
- `APIError` envelope on failure; `X-RateLimit-Remaining` header on every response.

## Steps
1. **Lock the draft for translation.** `PUT /drafts/{draftId}/lockForTranslation` (`lockDraftForTranslation`) — freezes source content so translations stay consistent (draft `status` becomes `LOCKED_FOR_TRANSLATION`).
2. **Discover translatable keys.** `GET /drafts/{draftId}/localizationKeys` (`getDraftLocalizationKeys`).
3. **List / create localizations.** `GET /drafts/{draftId}/localizations` (`getLocalizationForDraft`); create or update a language variant with `PUT /drafts/{draftId}/localizations/{languageId}` (`saveLocalization`).
4. **Set translations.** Read existing strings with `GET /drafts/{draftId}/localizations/{languageId}/translations` (`getTranslations`); write them with `PUT /drafts/{draftId}/localizations/{languageId}/translations` (`setTranslation`). Translation endpoints also accept/return gettext PO files.
5. **Clean up.** Remove a variant with `DELETE /drafts/{draftId}/localizations/{languageId}` (`deleteLocalization`).
6. **Unlock.** When translation is done, `DELETE /drafts/{draftId}/lockForTranslation` (`unlockDraftForTranslation`) to resume editing.

## Notes
- Translation lifecycle transitions emit `template_locked_for_translation` / `template_unlocked_for_translation` webhooks.

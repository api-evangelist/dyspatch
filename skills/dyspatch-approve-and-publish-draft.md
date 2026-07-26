---
name: Move a Dyspatch draft through approval
description: >-
  Take a Dyspatch draft through the review workflow — submit for approval,
  approve or reject, duplicate, or archive it. Use when automating the editorial
  approval lifecycle for email/SMS/push/voice content.
api: openapi/dyspatch-openapi-original.json
operations:
- getDrafts
- getDraftById
- submitDraftForApproval
- approveDraft
- approveDraftForAll
- rejectDraft
- duplicateDraft
- archiveDraft
---

# Move a Dyspatch draft through approval

Drive a draft through Dyspatch's approval workflow.

## Auth & conventions
- `Authorization: Bearer <DYSPATCH_API_KEY>` (needs a read & write key).
- `Accept: application/vnd.dyspatch.2026.06+json`.
- Cursor pagination on list endpoints; `APIError` envelope on failure; `X-RateLimit-Remaining` on every response.

## Steps
1. **Locate the draft.** `GET /drafts` (`getDrafts`) — filter by `templateId` if you know the template. Read `GET /drafts/{draftId}` (`getDraftById`) to check the draft `status`.
2. **Submit for approval.** `POST /drafts/{draftId}/publishRequest` (`submitDraftForApproval`).
3. **Approve or reject.**
   - Approve for the current group: `POST /drafts/{draftId}/publish/approve` (`approveDraft`).
   - Approve for all groups: `POST /drafts/{draftId}/publish/approveAll` (`approveDraftForAll`).
   - Reject: `POST /drafts/{draftId}/publish/reject` (`rejectDraft`).
4. **Duplicate or archive as needed.** `POST /drafts/{draftId}/duplicate` (`duplicateDraft`) to branch a copy; `DELETE /drafts/{draftId}` (`archiveDraft`) to archive.

## Notes
- Publishing and approval transitions emit webhooks (`template_submitted`, `template_approved`, `template_published`, …) — see `asyncapi/dyspatch-webhooks.yml` to react to them.
- Draft `status` uses `LOCKED_FOR_TRANSLATION` when locked for translation (renamed from `awaitingTranslation` in 2026.06).

---
name: Render a published Dyspatch template
description: >-
  Fetch a published Dyspatch template and render it to HTML with data, optionally
  in a specific language. Use when an application needs the final message body for
  a given template and recipient context.
api: openapi/dyspatch-openapi-original.json
operations:
- getTemplates
- getTemplateById
- renderTemplate
- renderTemplateByLCID
---

# Render a published Dyspatch template

Produce a ready-to-send message body from a published Dyspatch template.

## Auth & conventions
- Send `Authorization: Bearer <DYSPATCH_API_KEY>` on every request.
- Send `Accept: application/vnd.dyspatch.2026.06+json` to pin the API version.
- Watch the `X-RateLimit-Remaining` response header; on `429` (RateLimited) back off and retry.
- Errors return an `APIError` object (`code`, `message`, `parameter`).

## Steps
1. **Find the template.** `GET /templates` (`getTemplates`) — optionally filter by `name`, `folderId`, or `workspaceId`. Page with the `cursor` query parameter. Capture the `templateId`.
2. **(Optional) Inspect it.** `GET /templates/{templateId}` (`getTemplateById`) to confirm the template's variables and metadata before rendering.
3. **Render.** `POST /render/template/{templateId}` (`renderTemplate`) with a JSON body supplying the template's variables (see `variables` in the template response, and `customerprofiles` for named data sets). The response is the rendered body.
4. **Localized render (optional).** To render a specific language variant, call `POST /render/template/{templateId}/{languageId}` (`renderTemplateByLCID`) instead.

## Notes
- Only *published* templates render; drafts must be published first (see the create-and-publish skill).
- Supply an optional `themeId` where the endpoint accepts it to apply a specific design system.

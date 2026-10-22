# Better Notes legal pages

Static, dependency-free GitHub Pages site for Better Notes. Prepared from `memo-notes-app` commit `f4579d1` and provider documentation reviewed October 21, 2026.

## Before publishing (two required edits)

- Replace **[PUBLISHER LEGAL NAME]** in `privacy/index.html` with the correct legal publisher/operator name.
- Replace **[PUBLIC PRIVACY EMAIL]** and **[PUBLIC SUPPORT EMAIL]** in `privacy/index.html` and `support/index.html` with inboxes controlled by the operator. They can be the **same email address**.

The code and provider flow were researched; these are publisher decisions, not technical research tasks. Do not enable GitHub Pages or enter these URLs in App Store Connect until these fields are filled in and the account deletion workflow is deployed and tested.

## Publish

Go to this repository's **Settings → Pages → Build and deployment**, select **Deploy from a branch**, branch **main**, folder **/(root)**, and Save.

The URLs will be:
- https://aiden-hartman.github.io/better-notes-legal/
- https://aiden-hartman.github.io/better-notes-legal/privacy/
- https://aiden-hartman.github.io/better-notes-legal/support/

Check the URL in a private browsing window before setting:
- `EXPO_PUBLIC_PRIVACY_POLICY_URL=https://aiden-hartman.github.io/better-notes-legal/privacy/`
- `EXPO_PUBLIC_SUPPORT_URL=https://aiden-hartman.github.io/better-notes-legal/support/`

A public policy is part of launch readiness, not a replacement for the required in-app deletion and AI consent functionality.

## Audit notes

Actual app code uses Supabase (us-east-1), OpenAI, Foursquare Movement and Places, optional Hunter/Serper research, user-authorized HubSpot, Resend SMTP, and Expo EAS Updates. Telemetry is pruned locally on app start, seven days/ten sessions, while backend owner-scoped data remains until account deletion. Provider-side retention depends on their published terms/account settings; no uniform deadline is asserted.

Key sources:
- https://developers.openai.com/api/docs/guides/your-data
- https://docs.foursquare.com/developer/docs/movement-sdk-data-usage
- https://foursquare.com/legal/global-data-processing-addendum/
- https://supabase.com/legal/privacy-resources/data-residency-and-transfers-faq
- https://hunter.io/privacy-policy
- https://resend.com/security/gdpr
- https://expo.dev/privacy
- https://developer.apple.com/app-store/review/guidelines/

The policy is a factual, plain-language starting point; it should be reviewed for the operator's legal obligations and for changes in provider configuration before broad commercial rollout.

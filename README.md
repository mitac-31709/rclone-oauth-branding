# restic Home Backup — OAuth branding

Static homepage + privacy policy for the personal Google Cloud OAuth client used
by rclone / restic backups.

**App name must match the OAuth consent screen exactly:** `restic Home Backup`

## Live URLs (use these in GCP Branding)

- Home: https://restic-oauth.mitac.f5.si/
- Privacy: https://restic-oauth.mitac.f5.si/privacy.html
- Authorized domain: `mitac.f5.si`

Source also mirrors on GitHub Pages (not for GCP — ownership of `github.io` is
often rejected):

- https://mitac-31709.github.io/rclone-oauth-branding/

## Google Cloud Console checklist

1. [Search Console](https://search.google.com/search-console) → add **Domain**
   property `mitac.f5.si` → copy the DNS TXT record → add it in Cloudflare DNS
   for `mitac.f5.si` → Verify. Use the **same Google account** as the GCP project
   owner/editor.
2. Auth Platform → Branding:
   - App name: `restic Home Backup` (must match the homepage `<h1>`)
   - Home page: `https://restic-oauth.mitac.f5.si/`
   - Privacy policy: `https://restic-oauth.mitac.f5.si/privacy.html`
   - Authorized domains: `mitac.f5.si`
3. If ownership was just verified, wait up to **24 hours**, then request branding
   re-check with **「問題は修正した」** (the findings were correct — do not pick
   “issues are incorrect”).
4. Audience → Publish app (leave Testing).
5. `rclone config reconnect gdrive:` then `rclone about gdrive:`.

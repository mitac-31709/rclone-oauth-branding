# restic Home Backup — OAuth branding

Static homepage + privacy policy for the personal Google Cloud OAuth client used
by rclone / restic backups. **App name must match the OAuth consent screen
exactly:** `restic Home Backup`.

## Live URLs (Cloudflare Pages on owned domain)

- Home: https://restic-oauth.mitac.f5.si/
- Privacy: https://restic-oauth.mitac.f5.si/privacy.html
- Authorized domain (Search Console): `mitac.f5.si`

Fallback Pages.dev URL (not for GCP Branding — use the custom domain above):

- https://restic-oauth-branding.pages.dev/

## Google Cloud Console checklist

1. [Search Console](https://search.google.com/search-console) → verify **Domain**
   property `mitac.f5.si` (DNS TXT; same Google account as the GCP project).
2. Auth Platform → Branding:
   - App name: `restic Home Backup` (must match the `<h1>` on the homepage)
   - Home page: `https://restic-oauth.mitac.f5.si/`
   - Privacy policy: `https://restic-oauth.mitac.f5.si/privacy.html`
   - Authorized domains: `mitac.f5.si`
3. Wait up to 24 hours after domain verification, then request branding
   re-check with **「問題は修正した」** (not “issues are incorrect”).
4. Audience → Publish app (leave Testing).
5. `rclone config reconnect gdrive:` then `rclone about gdrive:`.

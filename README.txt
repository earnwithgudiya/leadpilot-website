LEADPILOT — SAFE UPDATE PACKAGE

CONTENTS
- index.html: updated single-file website.
- index.original-backup.html: untouched copy of the HTML you uploaded.
- supabase_activity_migration.sql: additive database migration for lead activity history.
- README.txt: deployment and testing notes.

WHAT THIS UPDATE CHANGES
1. Removes the duplicate sign-in click handler while retaining the existing Supabase email auth flow.
2. Corrects the GA4 loader ID to G-6XBQRVEFHE (matching the config ID already in your supplied file).
3. Removes hard-coded demo counts from the dashboard's initial HTML.
4. Adds an Activity History page. Once the SQL migration is run, Supabase records lead creation, edits and deletion automatically.
5. Makes the scoring and draft copy honest: current priority is rule-based and drafts are editable templates, not AI-generated content.

WHAT IT DOES NOT CLAIM
- No live AI generation is included. Do not put an AI provider secret key in browser code.
- No Gmail sending, WhatsApp, payment checkout, subscription entitlement, or scheduled reminders are included.
- This is not yet a fully production-ready commercial SaaS. Those require server-side functions, OAuth, verified payment webhooks, operational monitoring, backups, legal pages and testing.

DATA SAFETY
- The SQL migration creates a separate lead_activities table and triggers. It does not delete, truncate, rename or rewrite public.leads.
- Existing Supabase users, leads and RLS policies are not intentionally changed.
- Keep RLS enabled. Never paste a Supabase service_role/secret key into index.html.
- The included original-backup file is the exact HTML supplied for this update.

INSTALL
A. Website
1. Download and keep this ZIP as your rollback copy.
2. In GitHub, open the LeadPilot repository and upload the new index.html at the repository root, replacing the old index.html.
3. Do not upload index.original-backup.html as index.html. It is only a backup.
4. Commit the change and open the GitHub Pages site after deployment.

B. Activity history (optional but required for that page)
1. Open Supabase > SQL Editor > New query.
2. Open supabase_activity_migration.sql from this ZIP and copy all its contents.
3. Run it once. It adds a separate table and triggers; it does not modify existing lead rows.
4. Sign in to LeadPilot, add or edit a test lead, then open Activity history and tap Refresh.

TEST CHECKLIST
- Sign in with an existing account.
- Confirm your old leads still appear.
- Add a test lead, edit it, refresh the page and confirm persistence.
- Verify a second account cannot see the first account's leads.
- Test CSV export.
- If activity migration is installed, verify create/update/delete activity entries.
- Do not use confidential customer data until you have completed your own security and production review.

IMPORTANT
The source files supplied do not include a deployed backend/Edge Function for AI, Gmail, payments or scheduled automation. This package does not invent those integrations or pretend they are live.

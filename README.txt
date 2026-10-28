LEADPILOT — CLIENT-TESTING PROTOTYPE

Files
- index.html: responsive marketing site + interactive browser demo.

What you can test now
- Mobile-friendly landing page with a problem-focused value proposition.
- Demo dashboard: add/edit/delete sample leads, search/filter, see follow-up queue, view message draft starters, export CSV.
- Simple monthly admin-time cost calculator (illustrative estimate only).
- Proposed pricing interest form that opens a draft email.

Important limitations
This is NOT yet a production SaaS. There is no real signup/login, secure multi-user cloud database, Google Sheets OAuth/sync, live AI API, automatic email sending, payment checkout, subscription management, cancellation/billing portal, or hosted form submission. Demo data is stored in the visitor's browser only. The form opens an email draft and does not send or save data online. Do not enter real customer personal data.

Before charging customers
1. Interview target users and observe whether the demo solves a frequent, expensive problem.
2. Build secure authentication and per-user/team database access.
3. Implement and test Google Sheets/CSV import, live AI drafts with protected server-side API keys, and reliable reminders.
4. Add a payment provider with subscription creation, webhooks, billing portal, cancellation and refund/support terms.
5. Add privacy policy, terms, security checks, data deletion/export, and support contact.
6. Run a small pilot; only describe features as available after they work end-to-end.

Deploy
Upload index.html to the root of the GitHub repository and enable GitHub Pages from branch main / root, or import the repository into Netlify.

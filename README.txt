LEADPILOT V4 — INTERACTIVE FRONT-END PROTOTYPE

FILES
- index.html: single-file responsive prototype.
- README.txt: this guide.

WHAT WORKS IN THIS PROTOTYPE
- Responsive dark SaaS interface with Overview, Lead Pipeline, Follow-up Queue, Draft Studio, Analytics, Capabilities, and proposed Pricing pages.
- Add, edit, delete, search and filter leads.
- Change lead stage.
- Rule-based sample priority score (not AI).
- Due/overdue follow-up queue.
- Template-based editable follow-up draft preview, copy and download.
- CSV import/export.
- Browser localStorage persistence on the same browser/device.
- Proposed $19/$49/$99 monthly plans shown for planning only.

IMPORTANT LIMITATIONS — NOT A PRODUCTION SAAS
- No real AI API connection.
- No login, cloud database, multi-user access, tenant isolation, or server-side security.
- No Gmail or Google Sheets integration.
- No payment checkout, subscription verification, or plan entitlement controls.
- Demo data stays in the browser and may be lost if browser storage is cleared. Do not enter confidential or real customer data.
- Pricing is proposed only; the page explicitly says checkout is not connected.

DEPLOY
For a GitHub Pages static demo, replace the existing index.html with this index.html. Keep a copy of the previous file first. If uploading via phone, upload index.html at the repository root and commit the change. The README can also be uploaded at the root. GitHub Pages is appropriate for a non-commercial demo/portfolio, not as the production host for a commercial SaaS.

NEXT PRODUCTION WORK (NOT INCLUDED IN THIS ZIP)
1. Select a commercial-appropriate hosting/backend architecture.
2. Implement authentication and per-customer database access controls.
3. Implement server-side AI requests; never expose API keys in browser JavaScript.
4. Implement OAuth and secure Gmail/Sheets integrations.
5. Implement payment-provider checkout and server-side webhook verification before unlocking subscriptions.
6. Add privacy policy, terms, cancellation/refund details, support contact, monitoring and backups.

## Delivery Goal: Evergreen Quote Launch

### Goal

Deliver a production-ready Evergreen Quote experience that connects the React client, Express API, and MongoDB so customers can accurately create, save, and retrieve insurance quotes through a tested, containerized, and deployable solution.

### "Done" looks like

- The quote page loads its recent quotes from the API, and a saved quote survives a reload.
- The estimate on screen and the saved premium agree, at the launch rates.
- npm test (API) and npm run type-check + npm run build (client) pass; both CI jobs on the merge commit are green.
- The containerized API serves the wired app, and the cluster demo shows three API pods behind one Service.
- The landing page carries the launch banner and points at the app.
- A reviewed PR is merged, branch deleted.
- delivery-leadership-package/ is complete and committed.

### Out of scope (this week)

- Customer account management
- Policy purchasing workflows
- Production cloud hosting
- Advanced analytics and reporting
- Mobile applications
- Additional insurance products outside the supplied requirements
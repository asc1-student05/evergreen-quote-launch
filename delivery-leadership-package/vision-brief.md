## Evergreen Quote: Vision Brief

### Product

**Name:** Evergreen Quote Launch

**Delivery week:** Final

**Delivery Lead:** Jyoti Kumari

**Engineering team (represented by):** Evergreen Quote Launch Team

**GitHub Project board:** [Evergreen Quote Launch Delivery Board](https://github.com/users/asc1-student05/projects/5)

### Who is the customer?

The primary customer is an insurance shopper who wants a quick quote before speaking with an agent. They are typically comparing options online and expect immediate feedback about potential coverage costs. Today, their alternative is filling out forms, waiting for an agent response, or repeatedly entering the same information across multiple websites. These customers value speed, transparency, and confidence that the information they enter will be saved and available when they return.

### What pain does Evergreen Quote remove?

Customers become frustrated when they spend time entering quote information only to lose it after refreshing a page or when estimated pricing differs from what is ultimately saved. Evergreen Quote removes that friction by connecting the user interface directly to the backend service and database. Customers receive consistent pricing, can save quotes with confidence, and can return to see their information persist instead of starting over. This creates a more reliable and trustworthy quoting experience.

### What does "good" look like at end of the week?

- Recent quotes displayed in the application are retrieved from the API rather than local sample data.
- A customer can create and save a quote that remains available after refreshing the browser.
- The displayed estimate matches the premium stored by the backend service.
- API tests, client type checks, client build validation, and CI pipelines all pass successfully.
- The application is deployed through a containerized API and demonstrated running in Kubernetes with multiple API instances.

### What are we explicitly NOT doing this week?

- Building customer authentication or user account management.
- Implementing payment processing or policy purchasing functionality.
- Creating a production-grade cloud deployment.
- Redesigning the user interface beyond required launch updates.
- Adding new insurance products outside the provided Auto, Home, and Life quote capabilities.

### How will we know if it worked?

- 100% of demo quotes persist after browser refresh.
- All required CI jobs complete successfully with green status.
- API tests pass with no regression failures.
- Kubernetes deployment successfully runs three API pods behind a single service.
- End-to-end demo completes without manual data correction or application errors.
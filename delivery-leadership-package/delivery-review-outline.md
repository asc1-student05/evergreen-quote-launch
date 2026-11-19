## Program Showcase: Evergreen Quote Launch

### Slide 1: Delivery Goal & Did We Hit It?

Goal:
Deliver a production-ready Evergreen Quote experience that connects the React client, Express API, and MongoDB so customers can accurately create, save, and retrieve insurance quotes through a tested, containerized, and deployable solution.

Hit? ☒ Yes  ☐ Partially  ☐ No

Why:
Successfully connected the React application to the API and MongoDB, enabled GraphQL access, containerized the API, deployed to Kubernetes, validated deployment in Amazon EKS, and established CI/CD validation.

---

### Slide 2: What Shipped

- React quote application connected to live API data.
- MongoDB persistence enabled for saved quotes.
- Landing page updated with launch branding and quote links.
- GraphQL endpoint enabled and validated.
- Dockerized API image (evergreen-quote-api:2.0).
- Kubernetes deployment validated locally using Kind.
- GitHub Actions CI workflow enabled.
- Amazon EKS deployment completed and verified.
- Production-ready application with automated validation.
- Link to merged Pull Request.
- Link to green CI run.
- Screenshots of EKS deployment.

---

### Slide 3: Two Key Decisions

Decision 1:
Protect launch scope by approving marketing content updates while deferring Renters coverage and routing Auto-to-Life application changes for engineering review.

Why it mattered:
Prevented launch-week scope creep and reduced release risk.

Decision 2:
Issue a GO recommendation after Inject #2 because the verified launch environment remained healthy.

Why it mattered:
Focused decisions on evidence from the actual launch environment rather than an affected shared environment.

---

### Slide 4: Risks & Injects

Top Risks Tracked

- Launch-week scope creep.
- Environment configuration differences.
- Shared environment instability.
- Local demo readiness.

Inject #1 (Tuesday)

Situation:
Marketing requested Life-first messaging, Auto-to-Life default coverage, and Renters coverage.

Actions:
- Approved landing page content updates.
- Routed Auto-to-Life default change through engineering review.
- Deferred Renters coverage until after launch.

Outcome:
Protected launch scope while supporting business priorities.

Inject #2 (Wednesday)

Situation:
Shared demo environment reported "Could not load recent quotes."

Investigation:
- MongoDB remained healthy.
- API pods were restarting.
- Environment variable mismatch identified.

Actions:
- Routed issue to Platform Team.
- Communicated status to stakeholders.
- Validated local environment health.
- Completed Go / No-Go evaluation.

Outcome:
GO recommendation issued based on healthy local deployment and successful CI validation.

---

### Slide 5: End-to-End Delivery Journey

Phase 1:
Static Evergreen Insurance marketing landing page with launch branding.

Phase 2:
Typed React application with quote calculations and client-side validation.

Phase 3:
Express API, MongoDB persistence, GraphQL, Docker containerization, Kubernetes deployment, GitHub Actions CI/CD, and Amazon EKS deployment.

Copilot Experience:
- Assisted with implementation and troubleshooting.
- Identified additional impacted files.
- Updated implementation details and comments.
- Accelerated delivery activities.
- All generated changes were reviewed and validated before acceptance.

What I Take Back To Work:
Reliable delivery comes from clear ownership, scope management, automation, validation, and evidence-based decision making.

What I Would Do Differently:
Introduce deployment validation and environment-comparison testing earlier in the delivery lifecycle.

---

### Q&A Preparation

Q: Why didn't you ship Renters coverage?

A:
It introduced changes across the client, API, validation, and data model and represented unnecessary launch-week risk.

Q: Why did you recommend GO despite Inject #2?

A:
The issue was isolated to the shared demo environment. The validated launch environment, CI pipeline, Kubernetes deployment, and EKS deployment remained healthy.

Q: What value did Copilot provide?

A:
Copilot accelerated implementation, identified related files requiring updates, generated useful code suggestions, improved comments, and helped speed up troubleshooting while still requiring human review and validation.

Q: What technologies were demonstrated?

A:
React, TypeScript, Express, MongoDB, GraphQL, Docker, Kubernetes (Kind), GitHub Actions CI/CD, and Amazon EKS.

Q: What was the biggest leadership takeaway?

A:
Separate business requests from engineering changes, manage scope carefully, communicate ownership clearly, and make decisions based on verified evidence.
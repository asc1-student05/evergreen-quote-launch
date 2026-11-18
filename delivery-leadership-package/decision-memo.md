## Decision Memo: Launch Week Change Control and AI-Assisted Development

Date: Wednesday
Author: Jyoti Kumari
Decision Area: Launch readiness, scope control, and responsible use of AI tools

### Context

During launch week, Marketing requested Life-first messaging, a default coverage change from Auto to Life, and consideration of Renters coverage. At the same time, the team completed API integration, containerization, Kubernetes deployment, CI/CD setup, and launch preparation activities. Copilot was used to assist with development tasks and generated code updates, comments, and supporting changes across multiple files. The challenge was determining which changes should be accepted immediately and which should be reviewed or deferred to protect launch readiness.

### Options Considered

- **Option A: Accept all requested and AI-generated changes immediately.**
  - Pros: Faster delivery and maximum stakeholder satisfaction.
  - Cons: Increased launch risk, additional testing requirements, and potential introduction of unintended changes.

- **Option B: Accept business-content updates, validate Copilot-generated changes, and defer non-essential feature requests.**
  - Pros: Supports stakeholder objectives while maintaining quality, ownership, and launch stability.
  - Cons: Some requested enhancements are postponed until after launch.

- **Option C: Freeze all changes until after launch.**
  - Pros: Lowest change risk.
  - Cons: Misses opportunities to improve launch messaging and demonstrate responsiveness to stakeholders.

### Recommendation

Choose Option B. Approve landing-page content updates, validate all Copilot-generated code and comment changes before accepting them, route application behavior changes to the engineering team for review, and defer Renters coverage until after launch. This approach balances stakeholder expectations with delivery stability and protects the launch commitment.

### Why

The highest business priority is a successful and reliable launch. AI-generated changes can accelerate delivery, but all generated output must still be reviewed, tested, and validated before becoming part of a release. Launch readiness is more valuable than delivering additional unverified functionality.

### Trade-Offs

- Gained faster implementation through Copilot assistance.
- Increased review effort to validate generated changes.
- Accepted marketing content updates.
- Deferred non-essential functionality to reduce launch risk.
- Preserved schedule and delivery confidence while still responding to stakeholder requests.

### What Would Change My Mind

If engineering review, testing, CI validation, and stakeholder approval confirmed additional requested changes could be implemented safely without impacting launch readiness, those items could be reconsidered for inclusion before release.
## Decision Memo: Launch Week Change Control and AI-Assisted Development

Date: Wednesday
Author: Jyoti Kumari
Decision Area: Scope Control, Launch Readiness, and AI-Assisted Delivery

### Context

During launch week, Marketing requested changes to support a Life-first launch message, including changes to landing-page content, changing the default quote type from Auto to Life, and adding Renters coverage. At the same time the team was completing API integration, GraphQL enablement, Docker containerization, Kubernetes deployment, CI/CD implementation, and launch preparation activities.

Copilot was used during implementation and successfully generated updates across multiple files, identified related dependencies, suggested code changes, and improved comments and documentation. All generated changes were reviewed and validated before acceptance.

### Options Considered

#### Option A – Accept all requests and generated changes immediately

Pros:
- Maximum responsiveness
- Fast delivery

Cons:
- Increased launch risk
- Additional testing effort
- Potential unintended side effects

#### Option B – Accept content changes, review generated code, and defer non-essential features

Pros:
- Supports stakeholder priorities
- Maintains launch quality and stability
- Preserves delivery commitments

Cons:
- Some requests postponed until after launch

#### Option C – Freeze all changes until after launch

Pros:
- Lowest risk

Cons:
- Reduced responsiveness to stakeholder needs
- Missed opportunity to improve launch messaging

### Recommendation

Choose Option B.

- Approve landing page content updates.
- Review and validate all Copilot-generated changes before acceptance.
- Route application behavior changes to engineering ownership.
- Defer Renters coverage until after launch.

### Decision

Approved:

- Launch banner updates
- Landing page messaging updates
- Copilot-assisted implementation changes after validation

Deferred:

- Renters coverage

Routed for Engineering Review:

- Auto → Life default quote selection change

### Why

The primary objective is a stable, launch-ready solution. Every code change, whether human-written or AI-generated, requires validation before release. The team received the benefits of AI acceleration while maintaining change control and launch quality.

### Trade-Offs

Benefits:

- Faster implementation through Copilot assistance
- Improved productivity
- Faster identification of impacted files
- Better documentation and comments

Costs:

- Additional review effort
- Time spent validating generated output
- Some stakeholder requests delayed until after launch

### Outcome

The project successfully achieved:

- React Client → API integration
- MongoDB persistence
- GraphQL enablement
- Docker containerization
- Kubernetes deployment
- CI/CD validation
- Launch readiness review

### What Would Change My Mind

Additional functionality could be added before launch if:

- Engineering review confirms low risk
- CI remains green
- Required testing is completed
- Launch readiness is not impacted

## Risk Register

<table>
<tr>
<th>#</th>
<th>Risk</th>
<th>Owner</th>
<th>Likelihood (L/M/H)</th>
<th>Impact (L/M/H)</th>
<th>Mitigation</th>
<th>Trigger to escalate</th>
</tr>

<tr>
<td>R1</td>
<td>Client and API contract mismatch causes quote data to display incorrectly or fail during save operations.</td>
<td>Jyoti</td>
<td>M</td>
<td>H</td>
<td>Run npm run type-check, verify API responses using curl, and test quote creation after each integration change.</td>
<td>Type-check fails or quote save functionality breaks for more than one hour.</td>
</tr>

<tr>
<td>R2</td>
<td>MongoDB connectivity issues prevent quotes from being persisted and surviving page refreshes.</td>
<td>Jyoti</td>
<td>M</td>
<td>H</td>
<td>Verify MongoDB connection before testing, monitor API logs, and validate persistence through refresh testing.</td>
<td>Saved quotes disappear after refresh or database connection errors appear in logs.</td>
</tr>

<tr>
<td>R3</td>
<td>Docker image builds successfully but fails when deployed to Kubernetes due to configuration differences.</td>
<td>Jyoti</td>
<td>M</td>
<td>H</td>
<td>Test container locally before deployment and validate application functionality inside the running container.</td>
<td>Pods repeatedly restart, enter CrashLoopBackOff state, or fail readiness checks.</td>
</tr>

<tr>
<td>R4</td>
<td>CI pipeline failures delay pull request approval and final merge activities.</td>
<td>Jyoti</td>
<td>M</td>
<td>M</td>
<td>Run all local tests and builds before each push and review GitHub Actions results immediately after commits.</td>
<td>Any CI job remains red after two consecutive troubleshooting attempts.</td>
</tr>

<tr>
<td>R5</td>
<td>Scope creep from additional enhancements reduces time available for mandatory capstone deliverables.</td>
<td>Jyoti</td>
<td>H</td>
<td>M</td>
<td>Prioritize required lab objectives, track decisions in the project board, and defer non-required features.</td>
<td>Mandatory deliverables are incomplete within one day of the scheduled milestone.</td>
</tr>

</table>

### How I'll use this register

I will review this register during the start and end of each working session and update it whenever a new risk is identified or an existing risk changes. The register will be stored in the repository with the delivery leadership package so that instructors, reviewers, and project stakeholders can view the current risk status. Risks will be discussed during daily check-ins and escalated immediately when a trigger condition is met.

# External Service Troubleshooting Guide

**Purpose:** A general, reusable checklist for investigating external dependencies consumed by GraphQL integrations. This is a **public educational guide**, separate from existing restricted team documentation.

## 1. Identify the failure

- Record the GraphQL operation, environment, observable error, and approximate time.
- Determine whether the problem is repeatable.
- Do not copy customer data, secrets, credentials, or sensitive request payloads into public records.

## 2. Identify the system boundary

- Trace the call from the resolver through the service layer to the external dependency.
- Compare the expected response contract with the observed status and payload shape.
- Distinguish application mapping problems from failures originating upstream.

## 3. Reproduce safely

- Use only approved development or QA environments and sanitized test inputs.
- Check the happy path, missing/empty response, timeout, and relevant failure cases.
- Document what could be reproduced and what remains uncertain.

## 4. Extend one step

- Check **only the most directly related integration(s)** for the same known failure pattern.
- Document positive or negative results. A negative result is useful; it does not prove every integration is healthy.
- Stop the extension if it would require unauthorized access or expand beyond a bounded investigation.

## 5. Communicate ownership

- Identify which team owns the failed dependency and who owns the GraphQL integration.
- Explain observed impact, investigation evidence, and next decision in a findable, approved ticket.
- Do not conflate an investigation with a fix deployed by another team.

## 6. Verify and close

- Once an authorized fix is available, rerun affected tests with realistic *synthetic* data.
- Review response times and error counts when those measurements are available.
- Document: **Context; What I did; Why; Result; Notes for whoever is next**.
- Close only with a supported statement of what is resolved and what still depends on others.

## Example closing comment (educational)

> **Context:** A GraphQL operation experienced failures from a downstream dependency.  
> **What I did:** Reproduced the affected call in QA, collected sanitized evidence, and checked a closely related integration for the same pattern.  
> **Result:** The original failure was identified; no additional related integration issue was found during the bounded check. This is not proof that the external defect was corrected.  
> **For whoever is next:** Coordinate with the owning service team and validate the impacted operation after its fix is available.

## Constraints

Respect client policy, data boundaries, and service ownership. Do not add broad retries, change public API contracts, mask errors, or bypass access controls without authorization.

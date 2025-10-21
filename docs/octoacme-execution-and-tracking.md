# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
  - **Scrum Master:** Facilitates standup, tracks blockers, ensures time-boxing
  - Team members share progress and flag impediments
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone
  - **Scrum Master:** Facilitates demo, ensures stakeholder attendance
  - Team demonstrates completed work for feedback

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)
- **DevOps responsibilities:**
  - Maintain CI/CD pipelines for automated testing and deployment
  - Configure release gating (e.g., required checks, approvals)
  - Monitor deployment health and alert on failures
  - Provide runbooks for common deployment scenarios

## Quality & Testing
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI
- Manual QA for feature acceptance when needed
- **UX validation:**
  - Verify design fidelity during development and in QA
  - Conduct usability testing for major features
  - Validate accessibility standards (WCAG)
  - Sign off on UX acceptance criteria before release

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
- Level 1: Team-level triage in daily standup
  - **Scrum Master** works with team to identify and remove blockers
- Level 2: PM escalates to Product Lead and dependent teams
- Level 3: Sponsor-level escalation for business-impacting issues

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly

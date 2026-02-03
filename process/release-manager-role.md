# Release Manager – Role Description & Responsibilities

## Role Overview

The Release Manager is responsible for coordinating, overseeing, and executing the project's release process from initial planning through post-release follow-up.

This role ensures that each release meets quality, security, documentation, and communication standards, as defined in the project's [Release Checklist](/process/release-checklist.md), and that contributors are aligned throughout the process.

The Release Manager does not necessarily perform all tasks personally, but is accountable for ensuring they are completed, documented, and verified.

## Primary Responsibilities

### 1. Release Planning & Scoping

- Define and communicate release scope, versioning, and target timelines
- Coordinate with maintainers and contributors to identify included features, fixes, and breaking changes
- Ensure regulatory, licensing, and compliance considerations are reviewed when applicable
- Maintain and publish the release schedule

**Related checklist phases:** Pre-Release Planning – Release Scope & Timing

### 2. Process Coordination & Tracking

- Own and maintain the Release Checklist for each release
- Track progress across all release phases
- Identify blockers, risks, and dependencies early
- Ensure open items are assigned and followed up

**Related checklist phases:** All phases

### 3. Quality, Security, & Compliance Oversight

- Verify that testing, reviews, and validation steps are completed
- Ensure security scanning, SBOM generation, and compliance checks are performed
- Confirm that performance, stability, and upgrade paths meet project standards
- Escalate unresolved quality or security concerns

**Related checklist phases:** Development & Testing, Security & Compliance, Pre-Release Verification

### 4. Release Artifact & Branch Management

- Coordinate creation and verification of release builds and packages
- Ensure artifacts are signed, checksummed, and uploaded correctly
- Oversee tagging, branching, and versioning in the repository

**Related checklist phases:** Release Artifact Preparation, Release Execution – Distribution

### 5. Documentation & Communication

Coordinate preparation and review of:
- Release notes
- Changelog updates
- Migration/upgrade guides
- Security advisories

Ensure announcements are drafted and scheduled. Coordinate with communications and community leads as needed.

**Related checklist phases:** Documentation, Communications Preparation, Release Execution – Announcements

### 6. Release Execution

- Lead and coordinate day-of-release activities
- Confirm that all publication steps are completed
- Ensure releases are published across all official channels
- Validate that documentation and websites are updated

**Related checklist phases:** Release Execution

### 7. Post-Release Monitoring & Follow-Up

- Monitor issues, feedback, and metrics following release
- Coordinate hotfixes or patch releases if required
- Organize post-release retrospectives
- Update documentation and processes based on lessons learned
- Archive release artifacts and records

**Related checklist phases:** Post-Release – Monitoring, Post-Release – Follow-up

## Collaboration & Authority

### Works Closely With

- Maintainers and core contributors
- Security and compliance leads (if applicable)
- Documentation and communications teams
- Community moderators and support channels

### Authority

The Release Manager is empowered to:
- Delay a release if critical checklist items are incomplete
- Escalate blockers to project leadership
- Request additional reviews or testing
- Recommend process improvements
- Set code freeze dates and approve exceptions
- Make go/no-go recommendations for release

## Expected Skills & Qualities

### Technical Skills
- Familiarity with the project's codebase and tooling
- Understanding of version control workflows (Git)
- Knowledge of build and release processes
- Comfort with command-line tools and automation

### Organizational Skills
- Strong project coordination and tracking abilities
- Attention to detail and risk awareness
- Ability to manage multiple parallel workstreams

### Communication Skills
- Clear written and verbal communication
- Ability to coordinate distributed contributors
- Comfortable facilitating discussions and making decisions
- Experience documenting processes and decisions

### Leadership Qualities
- Comfort making go/no-go recommendations
- Proactive problem identification and escalation
- Ability to balance quality standards with pragmatic timelines

## Getting Started as Release Manager

### Prerequisites
- Active project contributor with demonstrated commitment
- Familiarity with the project's development workflow
- Understanding of the Release Checklist
- Nominated by existing maintainers or self-nomination accepted

### Onboarding Process
1. Shadow at least one complete release cycle
2. Co-manage a release with an experienced Release Manager
3. Review all release documentation and retrospectives
4. Obtain necessary access and credentials (see below)

## Tools & Access Requirements

The Release Manager needs access to:
- Repository write/admin access for tagging and branching
- Signing keys for release artifacts
- Distribution channel credentials (package registries, CDNs, etc.), if applicable
- Documentation site publishing access
- Communication channels (blog, social media, mailing lists)
- CI/CD system administrative access
- Issue tracker for creating milestones and tracking items

## Time Commitment

- **Planning phase:** 5-10 hours for scope definition and scheduling
- **Active development:** 2-5 hours per week monitoring progress
- **Release week:** 10-20 hours for final verification and execution
- **Post-release:** 5-10 hours for monitoring and retrospective
- Must be available and responsive during code freeze and release day

## Term & Rotation

- Release Managers may be appointed per release or serve for multiple release cycles
- The role may rotate among qualified maintainers to distribute responsibility
- Shadowing or co-managing releases is encouraged for knowledge transfer
- Release Managers may step down with appropriate notice to ensure continuity

## Support & Resources

### Documentation
- Release Checklist: [LINK](/process/release-checklist.md)
- Release Process Guide: [LINK](/process/release-process-guide.md)

## Notes

- Release schedules are targets—quality and security take precedence over deadlines
- Multiple people can share Release Manager duties or divide responsibilities
- First-time Release Managers should pair with experienced maintainers
- Document any deviations from standard process for future reference
- Regular retrospectives help continuously improve the release process

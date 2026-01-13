# Release Manager

## Overview

Release Managers are responsible for coordinating and executing releases across FAIR Package Manager projects. They ensure that releases follow the established [Release Calendar](./release-calendar.md) and adhere to the [Release Checklist](./release-checklist.md).

### Relationship to TSC

Release Manager is an **operational role** that is distinct from TSC membership:

- **TSC Members** provide governance, strategic direction, and approve major decisions (see [Organizers](../organizers.md))
- **Release Managers** handle the operational tasks of coordinating and executing releases

These roles may overlap:
- A TSC Member may also serve as a Release Manager
- A Release Manager does not need to be a TSC Member
- Release Managers report to the TSC on release status and process improvements

## Responsibilities

Release Managers are responsible for:

- **Release Coordination**: Coordinating release activities across working groups and projects
- **Quality Assurance**: Ensuring all pre-release checks and tests are completed
- **Artifact Management**: Building, signing, and publishing release artifacts
- **Documentation**: Maintaining release notes, changelogs, and upgrade guides
- **Communication**: Announcing releases and coordinating with the community
- **Process Improvement**: Identifying and implementing improvements to the release process
- **Compliance**: Ensuring releases meet security, licensing, and regulatory requirements

## Required Permissions

To perform their duties, Release Managers require the following permissions:

### GitHub Permissions

- **Write access** to all project repositories under the FAIR organization
- **Maintainer role** on GitHub teams managing release repositories
- **Admin access** to GitHub Actions and Workflows for CI/CD pipelines
- **Permission to create releases** and publish packages
- **Access to GitHub Packages** for publishing artifacts
- **Permission to manage tags** and protected branches
- **Access to repository secrets** needed for signing and publishing

### Infrastructure Access

- **CI/CD System Access**: Access to continuous integration and deployment systems
- **Package Registry Access**: Credentials for npm, Packagist, or other package registries
- **Code Signing Keys**: Access to GPG keys or other signing mechanisms
- **CDN/Distribution Access**: Permissions to upload and manage release artifacts
- **Documentation Platform**: Access to update release documentation

### Communication Channels

- **Announcement Permissions**: Ability to post announcements on official channels
- **Slack Channel Access**: Admin or moderator access to release-related Slack channels
- **Mailing List Access**: Permission to send release announcements

## Current Release Managers

| Name | GitHub Handle | Projects | Term Start |
|------|---------------|----------|------------|
| _TBD_ | _TBD_ | _TBD_ | _TBD_ |

> **Note**: This list should be updated as Release Managers are added or removed.

## Adding a Release Manager

> **Note**: Release Manager is an operational role separate from TSC membership. A Release Manager may or may not be a TSC Member. TSC Members who wish to take on release responsibilities should follow the process below.

### Nomination Process

1. **Nomination**: Release Managers may be nominated by any TSC member or may self-nominate
   - TSC Members can volunteer to become Release Managers
   - Community contributors can be nominated by TSC members
2. **Criteria Evaluation**: Nominees should demonstrate:
   - Strong understanding of the FAIR release process and calendar
   - Experience with version control, CI/CD, and release workflows
   - Commitment to following established processes and checklists
   - Good communication skills and attention to detail
   - Availability during release windows
3. **TSC Approval**: The nomination must be approved by TSC consensus or vote
4. **Onboarding**: Once approved, the new Release Manager should be onboarded using the process below

### Technical Onboarding

After TSC approval, the following steps should be completed:

#### 1. GitHub Access
```bash
# Add the Release Manager to the GitHub teams
# This should be done by a GitHub organization owner
```

- Add to the `release-managers` GitHub team (create if it doesn't exist)
- Grant write access to all project repositories
- Add to relevant repository-specific teams as needed
- Verify access to GitHub Actions and Packages

#### 2. Infrastructure Access

- **Package Registries**: Create accounts and grant publishing permissions
  - npm: Add to the `@fairpm` organization with publisher role
  - Packagist: Grant submitter/updater permissions
  - Other registries as applicable
- **CI/CD Systems**: Grant access to CI/CD dashboards and configurations
- **Code Signing**: Provide or generate GPG keys for artifact signing
  - Document the key fingerprint in a secure location
  - Add public key to the project's keyserver
- **CDN/Distribution**: Grant upload permissions to release artifact storage

#### 3. Communication Access

- Add to `#releases` Slack channel with appropriate permissions
- Add to release announcement mailing lists
- Grant access to the release section of the website/documentation platform

#### 4. Documentation Review

The new Release Manager should review:
- [Release Calendar](./release-calendar.md)
- [Release Checklist](./release-checklist.md)
- [Release Names](./release-names.md)
- [Fair GitHub Management](./fair-github-management.md)
- Any project-specific release procedures

#### 5. Update Documentation

- Add the Release Manager to the [Current Release Managers](#current-release-managers) table
- Document any project-specific responsibilities
- Share credentials securely using the project's approved secrets management system

## Removing a Release Manager

### Offboarding Process

When a Release Manager steps down or needs to be removed:

#### 1. Transition Planning

- **Transfer Responsibilities**: Identify and reassign any in-progress releases
- **Knowledge Transfer**: Conduct handoff session with remaining Release Managers
- **Documentation Update**: Ensure all procedures and credentials are documented

#### 2. Access Revocation

Complete the following steps promptly to maintain security:

##### GitHub Access
- Remove from `release-managers` GitHub team
- Revoke write access to project repositories
- Remove from repository-specific teams
- Audit and revoke any personal access tokens (PATs)

##### Infrastructure Access
- **Package Registries**: Remove publisher permissions from npm, Packagist, etc.
- **CI/CD Systems**: Revoke access to CI/CD dashboards
- **Code Signing**: Revoke or rotate GPG keys if necessary
  - Document revoked key fingerprints
  - Update project documentation if keys are rotated
- **CDN/Distribution**: Remove upload permissions

##### Communication Access
- Remove from `#releases` Slack channel or downgrade permissions
- Remove from release announcement distribution lists
- Revoke website/documentation platform access

#### 3. Security Review

- **Credential Rotation**: Rotate any shared credentials the Release Manager had access to
- **Key Rotation**: Consider rotating code signing keys if appropriate
- **Audit Trail**: Document the offboarding in TSC records

#### 4. Update Documentation

- Remove the Release Manager from the [Current Release Managers](#current-release-managers) table
- Update any project-specific documentation that references the individual
- Archive any personal documentation or notes they maintained

## Emergency Procedures

### Temporary Access Revocation

If immediate access revocation is needed due to security concerns:

1. Contact GitHub organization owners immediately
2. Revoke GitHub access first (highest priority)
3. Rotate any compromised credentials
4. Follow the full offboarding process afterward
5. Notify the TSC of the incident

### Backup Release Managers

To ensure release continuity:

- Maintain at least **2-3 active Release Managers** at all times
- Cross-train Release Managers on all projects
- Document all procedures so any Release Manager can execute any release
- TSC Co-chairs should have emergency release capabilities

## Best Practices

- **Principle of Least Privilege**: Grant only the permissions necessary for the role
- **Regular Access Reviews**: Audit Release Manager permissions quarterly
- **Credential Management**: Use secure credential management systems (1Password, LastPass, etc.)
- **Two-Person Rule**: For critical releases, consider requiring two Release Managers to sign off
- **Documentation**: Keep this document updated as processes and tools evolve
- **Automation**: Automate permission management where possible using Infrastructure as Code

## Related Documentation

- [Release Calendar](./release-calendar.md)
- [Release Checklist](./release-checklist.md)
- [Release Names](./release-names.md)
- [Fair GitHub Management](./fair-github-management.md)
- [TSC Process Documentation](./README.md)

## Questions?

For questions about the Release Manager role or to nominate someone, please:
- Open an issue in the [TSC repository](https://github.com/fairpm/tsc/issues)
- Contact the TSC Co-chairs
- Post in the `#releases` Slack channel


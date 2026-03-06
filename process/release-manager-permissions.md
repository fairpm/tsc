# Release Manager Permissions

## Required Permissions

To perform their duties, Release Managers require the following permissions:

### GitHub Permissions

- **Write access** or higher to the release source repository
- **Maintainer role** or higher to `fairpm/tsc` repository
- **Permission to re-run existing workflows** in GitHub Actions (included in the Maintainer role)
- **Permission to create releases** and publish packages
- **Access to GitHub Packages** for publishing artifacts
- **Permission to manage tags** and protected branches

## Infrastructure Access (may be delegated)

Not all permissions need to be held personally by the Release Manager. Some steps — particularly cache flushing and infrastructure tasks — may be performed by a delegate (e.g., a DevOps or site administrator) at the Release Manager's coordination.

Access that may be required depending on the project:

- **AWS Console** — for flushing object/site caches (e.g., ElastiCache/Valkey)
- **WordPress network admin** — for clearing plugin update caches (e.g., Git Updater)
- **CDN access** — for purging edge caches (e.g., Fastly)

The Release Manager is responsible for ensuring these steps are completed, not necessarily for performing them directly.

## Managing the **Release Managers** team

A Release Managers team exists at the organization level. This team has `maintain` access to the `fairpm/tsc` repository.

### Add a Release Manager:

1. Go to the [Release Managers team](https://github.com/orgs/fairpm/teams/release-managers)
2. Click the *Add a member* button
3. Search for the user you wish to add to the team
4. Click the + sign next to the user and then click the **Invite** button

### Remove a Release Manager:
1. Go to the [Release Managers team](https://github.com/orgs/fairpm/teams/release-managers)
2. Select the member you wish to remove
3. Click **Remove from team**

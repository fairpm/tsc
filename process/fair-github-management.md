## Summary

This document outlines how the FAIR project organizes work using GitHub Projects.

## Repository Organization

Each workgroup should have a single project board, this enables:

- A single source of truth for the workgroup's backlog
- Focused discussion and issue tracking 
- Workgroup-specific processes (templates, automation, etc.)

## Cross-Workgroup Coordination

### Organization Roll-up 

For milestones that span multiple workgroups, FAIR uses an organization "roll-up" project that:

- Groups issues by milestone across all workgroup repositories
- Provides unified visibility of cross-team initiatives (e.g., V1.01 milestone)
- Automatically includes issues from workgroups based on milestone assignment

Issues are automatically added to the roll-up board when assigned to specific milestones using GitHub's [auto-add workflow](https://docs.github.com/en/issues/planning-and-tracking-with-projects/automating-your-project/adding-items-automatically). 

For cross-workgroup milestones, the TSC should establish consistent milestone names to ensure proper automation across workgroups.

## Recommended Best Practices

### Project Boards

Recommended columns are:

- Icebox → ideas/parked
- Backlog → accepted but not scheduled
- In Progress → actively being worked
- Review / QA → PR open or testing
- Done → closed/merged (auto-move on close)

Enable the built-in workflow rule: When issue/PR closes → move to Done.

### Labels

Recommended labels include:

- bug
- chore
- discussion
- documentation
- feature-request
- good-first-issue

Suggested additions to consider:

- blocked (for issues waiting on dependencies)
- help-wanted (for issues needing additional contributors)
- priority-high/medium/low (for triaging urgency)
- testing (for test-related work)

Feel free to expand as needed.

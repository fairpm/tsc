# The FAIR Package Manager: Team Lifecycle Policy

## Purpose

This document defines a process for proposing, approving, operating, and retiring teams under the FAIR Technical Steering Committee (TSC).  

Teams are autonomous initiatives created by the Technical Steering Committee (TSC) that fall into two categories:

- **Standing Teams**: Long-lived, self-sustaining teams with formal governance, charters, roadmaps, and dedicated maintainers. These teams operate continuously and manage ongoing aspects of the project (similar to committees like the TSC itself).

- **Initiative Teams**: Temporary, task-oriented teams formed to achieve specific outcomes or deliverables. These teams dissolve once their objectives are completed.

The TSC will periodically review each team to ensure it maintains the appropriate structure for its current needs.

## Team Categories

### Standing Teams

- Permanent or long-term duration
- Can have formal governance structure and charter
- Defined roadmap and ongoing responsibilities  
- Regular maintainers and contributors

### Initiative Teams  

- Time-bound or outcome-bound duration
- Focused on specific deliverables or tasks
- Lighter governance requirements
- Dissolve upon completion of objectives

## Proposing A New Team

- **Who Can Propose**  
  Any active contributor may propose the creation of a team.

- **Proposal Requirements**  
  Each proposal must include:
  1. Name / Title  
  2. Team Type (Standing or Initiative)
  3. Scope (what the team will address)  
  4. Objectives & Deliverables  
  5. Initial Membership (lead(s) and core participants)  
  <!--Future
  6. For Initiative Teams: Expected timeline and completion criteria
  7. For Standing Teams: Draft charter and governance model -->

- **Submission**  
  Proposals are filed as GitHub issues in the [`fairpm/tsc`](https://github.com/fairpm/tsc) repository with the label `team-proposal` and either `standing-team` or `initiative-team`.

## Review & Approval

- **Evaluation Criteria**  
  - Relevance to FAIR project goals  
  - Clarity of objectives  
  - Feasibility (time, scope, resources)  
  - Membership and leadership

- **Decision Process**  
  - The TSC reviews the proposal in a meeting or asynchronously via GitHub.  
  - A simple majority vote of those participating in the meeting or a GitHub discussion without unresolved objections is required for approval.   
  - Decision and rationale are documented in the proposal issue. 


## Operations & Tracking

- **Tracking Requirements**  
  
  **For Standing Teams:**
  - Published roadmap and regular status updates
  - Agendas, meeting notes, and deliverables discoverable via the team repo 
  - Work items tracked via GitHub issues and project boards
  - Quarterly reports to the TSC
  
  **For Initiative Teams:**
  - Completion criteria documented
  - Progress tracked via GitHub issues/project boards
  - Monthly status updates to the TSC
  - Final report upon completion

- **Communication**  
  Optional Slack channels or mailing lists may be created, but GitHub is the system of record.

## Reviews & Overall Lifecycle

### Standing Teams
- **Annual Review**  
  Each Standing Team should present an annual review to the TSC.

### Initiative Teams  
- **Progress Review**  
  Monthly check-ins with the TSC.
  
- **Extension**  
  If additional time is needed, teams can request an extension with updated timeline and rationale.
  
- **Completion**  
  Upon achieving objectives, Initiative Teams should:
  - Submit a final report documenting outcomes
  - Transfer any ongoing responsibilities to Standing Teams
  - Archive repositories and close project boards

### Both Team Types

- **Dormancy**  
  If a team is inactive for 3 months, it will be marked *Dormant* in the project README.  

- **Dissolution**  
  - Initiative Teams dissolve automatically upon completion
  - Standing Teams may be dissolved by TSC decision  
  - All dissolutions require:
    - Closing summary in the team's README
    - Repository archival
    - Transfer of any continuing responsibilities  

## Governance 

- All teams operate under the authority of the FAIR TSC and Technical Charter.  
- Each team should have a copy of the [`sample-readme.md`](https://github.com/fairpm/tsc/tree/main/teams/sample-readme.md) in their repo, expanded as needed.

All teams must:
- Follow TSC policies, including the Code of Conduct and Licensing policies
- Maintain accessible workspaces (Slack channels, forums, etc.) posted centrally
- Document how contributors can participate

A [sample meeting notes template](https://github.com/fairpm/tsc/tree/main/working-groups/sample-meeting-notes.md) is available.

## Active Standing Teams

### AspireCloud

The AspireCloud Team is responsible for the development and maintenance of AspireCloud, a standalone API server that acts as a bridge between a mirror of the legacy WordPress plugin repository and the emerging FAIR protocol ecosystem.

AspireCloud currently indexes a mirror of the WordPress.org plugin repository and exposes that data via a custom API. The group is now extending AspireCloud to support the FAIR protocol in addition to the traditional WordPress API, enabling unified search and discovery across both systems.

This work is seen as a critical transitional layer to support adoption of the FAIR Package Manager by maintaining compatibility with existing workflows while introducing a more modern and federated package model.

AspireCloud is built with Laravel and PostgreSQL.

### FAIR

The FAIR Team is responsible for the development and operation of The FAIR Package Manager, including server infrastructure, protocol design, and a connector plugin.

This includes the design of the decentralized protocol, design and operation of the discovery aggregator, design and operation of repository node software, and design and operation of the analytics service. These are as outlined in the previously-created Timeline and Goals document; specifically, Phase 3 (“MVP”), Phase 4 (“Distributed FAIR”), and Phase 5 (“Full FAIR”).

It also includes the installable connector plugin, which is expected to exist as a module within the plugin created by the Independence Team. The Independence Team will create the plugin initially, however long-term maintenance will transition to The FAIR Team upon that Team’s completion.


### Website Management

The Website Management Team is focused on building and maintaining the technical foundation of the FAIR Package Manager for WordPress project website and its wider network of related sites. This includes implementation frameworks, wireframes, accessibility, technical SEO, and scalable content architecture.

## Active Initiative Teams

### Community Initiative

The Community Initiative is a documentation and process-focused team supporting contributor onboarding and clarifying how to engage with the FAIR Package Manager project.

- [Community Initiative](./community/)
- **Expected Completion**: [To be defined]

## Past Teams

### Technical Independence

The Technical Independence Team is responsible for developing a solution to independence from the existing central WP server.

This includes a replacement central server, a plugin to connect existing WP sites to this server, and the creation of tools to package and maintain a distribution of WP including this plugin. These are as outlined in the previously-created Timeline and Goals document; specifically, Phase 1 (“Drop-In Mirror”) and Phase 2 (“Sever Connection”).

The plugin created by the Technical Independence Team is to be created in a modular way, so that the plugin and tooling can be used by The FAIR Team.

**The Technical Independence Team is time- and scope-limited to the development of this solution. Once the solution is created, long-term maintenance of the plugin and any server components will transition to The FAIR Team. The Technical Independence Team shall complete its work prior to June 5, aiming for May 5 for a usable MVP of its work.**

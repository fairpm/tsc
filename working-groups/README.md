# FAIR Project: Working Group Lifecycle Policy

## Purpose

This document defines a lightweight process for proposing, approving, operating, and retiring Working Groups under the FAIR Technical Steering Committee (TSC).  

Working Groups (“WGs”) are autonomous initiatives created by the Technical Steering Committee (TSC). Working groups are more fluid than projects and may dissolve once their goals are achieved.

The TSC will periodically review each WG to decide whether it should remain as a WG or adopt an alternative structure.

## Proposing A New Working Group

- **Who Can Propose**  
  Any active contributor may propose the creation of a WG.

- **Proposal Requirements**  
  Each proposal must include:
  1. Name / Title  
  2. Scope (what the group will address)  
  3. Objectives & Deliverables  
  4. Initial Membership (lead(s) and core participants)  
  5. Timeline or milestones (if applicable)  

- **Submission**  
  Proposals are filed as GitHub issues in the [`fairpm/tsc`](https://github.com/fairpm/tsc) repository with the label `wg-proposal`.

## Review & Approval

- **Evaluation Criteria**  
  - Relevance to FAIR project goals  
  - Clarity of objectives  
  - Feasibility (time, scope, resources)  
  - Membership and leadership

- **Decision Process**  
  - The TSC reviews the proposal in a meeting or asynchronously via GitHub.  
  - A simple majority vote is required for approval.  
  - Decision and rationale are documented in the proposal issue. 


## Operations & Tracking

- **Dedicated Repository**  
  Approved WGs will normally receive their own repository under the FAIR GitHub organization, named `wg-<name>` (e.g., `wg-docs`).  

- **Tracking Requirements**  
  - Agendas, meeting notes, status reports, and deliverables stored in the WG repo. 
  - Work items tracked via GitHub issues and project boards.  

- **Communication**  
  Optional Slack channels or mailing lists may be created, but GitHub is the system of record.


## Review & Sunset

- **Periodic Review**  
  Every 6 months, each WG must review its purpose, progress, and continued relevance.  

- **Dormancy**  
  If a WG is inactive for 3 months, it will be marked *Dormant*.  

- **Dissolution**  
  When objectives are complete or no longer relevant, the WG may be dissolved by consensus of its members or by TSC decision.  
  - Leads must post a closing summary in the README of the project.  
  - Repositories or project boards will be archived.  

---

## Governance 

- All working groups operate under the authority of the FAIR TSC and Technical Charter.  
- Each working group should have a copy of the [`sample-readme.md`](https://github.com/fairpm/tsc/tree/main/working-groups/sample-readme.md) in their repo, it can be expanded as needed.

Working Groups have a high degree of flexibility in how they work, but the following is required:
- All TSC policies, including the Code of Conduct and Licensing policies must be included by reference.
- Workspaces for all Working Groups, such as Slack channels, forums, mailing lists or other spaces must be posted centrally for easy access.
- All Working Groups must share details on how someone can contribute to them.

A [sample meeting notes template](https://github.com/fairpm/tsc/tree/main/working-groups/sample-meeting-notes.md) is available.

## Active Working Groups

### AspireCloud

The AspireCloud Working Group is responsible for the development and maintenance of AspireCloud, a standalone API server that acts as a bridge between a mirror of the legacy WordPress plugin repository and the emerging FAIR protocol ecosystem.

AspireCloud currently indexes a mirror of the WordPress.org plugin repository and exposes that data via a custom API. The group is now extending AspireCloud to support the FAIR protocol in addition to the traditional WordPress API, enabling unified search and discovery across both systems.

This work is seen as a critical transitional layer to support adoption of the FAIR Package Manager by maintaining compatibility with existing workflows while introducing a more modern and federated package model.

AspireCloud is built with Laravel and PostgreSQL.

**The AspireCloud WG is a permanent Working Group.**

### Community

The Community Working Group (CWG) is a documentation and process-focused initiative to support contributor onboarding and clarify how to engage with the FAIR Package Manager project.

- [Community WG](./community/)

### FAIR

The FAIR Working Group is responsible for the development and operation of The FAIR Package Manager, including server infrastructure, protocol design, and a connector plugin.

This includes the design of the decentralized protocol, design and operation of the discovery aggregator, design and operation of repository node software, and design and operation of the analytics service. These are as outlined in the previously-created Timeline and Goals document; specifically, Phase 3 (“MVP”), Phase 4 (“Distributed FAIR”), and Phase 5 (“Full FAIR”).

It also includes the installable connector plugin, which is expected to exist as a module within the plugin created by the Independence WG. The Independence WG will create the plugin initially, however long-term maintenance will transition to The FAIR WG upon that WG’s completion.

**The FAIR WG is a permanent Working Group.**

### Website Management

The Website Management Working Group is focused on building and maintaining the technical foundation of the FAIR Package Manager for WordPress project website and its wider network of related sites. This includes implementation frameworks, wireframes, accessibility, technical SEO, and scalable content architecture.

**The Website Management WG is a permanent Working Group.**

## Past Working Groups

### Technical Independence

The Technical Independence Working Group is responsible for developing a solution to independence from the existing central WP server.

This includes a replacement central server, a plugin to connect existing WP sites to this server, and the creation of tools to package and maintain a distribution of WP including this plugin. These are as outlined in the previously-created Timeline and Goals document; specifically, Phase 1 (“Drop-In Mirror”) and Phase 2 (“Sever Connection”).

The plugin created by the Technical Independence WG is to be created in a modular way, so that the plugin and tooling can be used by The FAIR WG.

**The Technical Independence WG is time- and scope-limited to the development of this solution. Once the solution is created, long-term maintenance of the plugin and any server components will transition to The FAIR WG. The Technical Independence WG shall complete its work prior to June 5, aiming for May 5 for a usable MVP of its work.**

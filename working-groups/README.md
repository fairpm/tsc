# The FAIR Package Manager - Working Groups

Working Groups (“WGs”) are autonomous projects created by the Technical Steering Committee (TSC).

Working Groups can be formed at any time but must be ratified by the TSC. Once formed the work defined in the Working Group charter is the responsibility of the WG rather than the TSC.

As the TSC Charter is intended as a temporary charter, any Working Groups formed under the charter are similarly temporary. When a permanent TSC Charter is created, any prior Working Groups must be ratified by the TSC under the terms of the new TSC Charter.

When the work defined in a Working Group's charter is complete, the charter will be dissolved (revoked) unless there is a reason to extend it to a permanent Working Group.

A Working Group's charter can be revoked either by consent of the Working Group's members or by a TSC vote. Once revoked, any future work that arises becomes the responsibility of the TSC.

## Starting A Working Group

A Working Group is established by the TSC, with a statement of purpose and a list of responsibilities. The list of responsibilities should be specific. Each Working Group is self-governed under the standard governance below.

## Governance Rules for Working Groups

The following is a temporary set of governance rules for each Working Group. It is the intention that under a future TSC Charter, working groups shall have the ability to self-govern.

Each Working Group should copy the [`sample-readme.md`](https://github.com/fairpm/tsc/tree/main/working-groups/sample-readme.md) file as a template and place it within their designated subfolder under `/working-groups/` in the this repository (e.g., `/working-groups/community/README.md`). This file serves as the project “front door” for the Working Group and should be customized with the relevant details in `{}`. If the Working Group operates from a separate repository, the file should instead be placed in that repository’s main README or equivalent homepage.

Working Groups have a high degree of flexibility in how they work, but the following should remain consistent across all groups:

* All TSC policies, including the Code of Conduct and Licensing policies must be included by reference;
* Workspaces for all Working Groups, such as Slack channels, forums, mailing lists or other spaces must be posted centrally for easy access;
* All Working Groups must share details on how someone can contribute to them;

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

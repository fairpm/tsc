## About the Website Management Working Group

The Website Management Working Group is focused on building and maintaining the technical foundation of the FAIR Package Manager for WordPress project website and its wider network of related sites. This includes implementation frameworks, wireframes, accessibility, technical SEO, and scalable content architecture.

This working group is hosted by The FAIR Package Manager for WordPress Technical Steering Committee (TSC).

We follow The FAIR Package Manager [Code of Conduct](../../code-of-conduct.md).

Organizer access to this group is granted to members of The FAIR Package Manager TSC and regular contributors to the project, as determined by The FAIR Package Manager TSC. To request access, please reach out to a TSC member.

This project is licensed under the GNU General Public License (GPL), v2 or later.

This group welcomes contributions from any member of our community. To get started contributing, please see the contribution guide on this repo.

This Working Group is intended to be evergreen. Its scope may evolve over time to meet the needs of the project and the direction set by the TSC.

## 🧱 Scope & Implementation Strategy
The Website Management Working Group will use the existing [`fair-parent-theme` repository](https://github.com/fairpm/fair-parent-theme) as its foundation. This theme is a fork of the lightweight and accessible [Air Light](https://airwptheme.com/) starter theme. While contributions may extend or adapt this base, rebuilding from scratch is not within scope.

A key responsibility of the group is to determine what functionality and content should live inside WordPress and what should remain external. The group will develop a clear architecture plan before implementation begins.

The goal is to create a clean, minimal site framework that can be reused across the network. The design layer will come later, but this foundation should be structurally flexible enough to support a wide range of branding and layout needs with minimal future customization.

Work will proceed in two major phases:

* Initial Rapid Phase – Launch a front-facing site quickly to improve visibility of existing documentation

* Longer-Term Architectural Phase – Focus on maintainable network-wide architecture, theme structure, and extensibility

All development using WordPress will occur within the existing WordPress multisite environment already provisioned for the project. No new infrastructure setup is needed for WordPress.

## Github Repositories
- https://github.com/fairpm/website-content
- https://github.com/fairpm/server
- https://github.com/fairpm/fair-parent-theme
- https://github.com/fairpm/fair-child-theme

## 📌 Current Tasks

### 🏃‍♂️ Initial Efforts

#### Launch Initial Public Site
Set up a front-facing site within the existing multisite that presents key project documentation in a clean, accessible format. This will act as the initial demonstration of the framework.

#### Finalize Initial Theme Configuration
Adapt the fair-parent-theme to suit immediate project needs. Ensure the theme supports flexible layouts, a clear content structure, and meets baseline accessibility and SEO expectations.

#### Define Content Architecture Plan
Decide what content and functionality belong within the WordPress environment and what should remain external. Document the architecture for implementation.

#### Wireframe Key Page Types
Create basic wireframes for core templates — including homepage, documentation hub, Working Group microsite, and future plugin directory — to guide development efforts.

### 🔄 Evergreen Responsibilities
* Maintain and evolve the theme framework to support project needs across the network
* Ensure all sites meet baseline accessibility and technical SEO standards
* Guide decisions on content architecture, including what content belongs where across the multisite network
* Provide input on HTML structure and template organization
* Collaborate with other Working Groups to support publishing needs without assuming responsibility for content writing or design

## ✅ Completed Tasks

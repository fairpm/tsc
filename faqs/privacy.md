# Frequently Asked Questions About Privacy and GDPR

---
status: "ongoing"
date: 2025-06-11
---

## What does FAIR track?

By default, the FAIR WordPress plugin tracks nothing. There are, however, services that the plugin uses to help support its features. You can read more about that in the plugin [Readme file](https://github.com/fairpm/fair-plugin/blob/main/README.md#data-privacy)

## How does FAIR impact user privacy?

FAIR is designed to improve user privacy by reducing unnecessary tracking and central data collection.

For example, avatars are generated locally instead of making remote calls. Health checks and package updates (like for plugins and themes) no longer sends telemetry metrics about individual sites.

This means less personal data is collected and stored, reducing the risk of data breaches and making it easier for site owners to comply with privacy law requirements. FAIR's approach ensures that only essential, anonymized data is used, and users have greater control over their information.

## How does FAIR support compliance with the GDPR?

FAIR's design works by minimizing data, maximizing user control, and reducing the complexity of legal obligations for site owners, helping site owners comply with several key GDPR requirements:

* Data Minimization (Article 5): FAIR reduces the amount of personal data collected and processed by eliminating unnecessary tracking and central telemetry. Only essential, anonymized data is used.
* User Consent (Articles 6, 7): By default, FAIR does not collect or transmit personal data for analytics or updates, reducing the need for complex consent mechanisms.
* Right of Access and Data Portability (Articles 15, 20): Since less personal data is collected and stored, it is easier for site owners to provide users with access to their data or export it if requested.
* Right to Erasure (Article 17): With minimal data collection, there is less data to erase, making it easier to honor user deletion requests.
* Transparency (Articles 12, 13): FAIR's privacy-first approach and decentralized architecture make it clear to users what data is (and isn't) collected, supporting transparency obligations.
* Security of Processing (Article 32): By decentralizing distribution and reducing central data storage, FAIR lowers the risk of data breaches and unauthorized access.

## How does FAIR support compliance with the California Consumer Privacy Act (CCPA)?

FAIR's architecture reduces the amount of personal data collected and shared, making it easier for site owners to meet several key CCPA requirements:

* Right to Know: FAIR minimizes the collection and sharing of personal information, making it easier for site owners to inform users about what data is collected, used, or disclosed.
* Right to Delete: With minimal data collection and no central telemetry, there is less personal information to delete, simplifying compliance with user deletion requests.
* Right to Opt-Out: FAIR's privacy-first design means there is no sale or sharing of personal data for analytics or advertising, reducing the need for complex opt-out mechanisms.
* Non-Discrimination: Since FAIR does not rely on user data for core functionality, site owners can honor privacy requests without penalizing users or degrading service.
* Transparency: FAIR's decentralized approach and clear documentation make it easy for site owners to provide users with accurate privacy notices and disclosures.

## How does FAIR support compliance with the EU Cyber Resilience Act (CRA)?

FAIR's design and architecture improves supply chain security and reduces attack surfaces, making it easier for site owners to comply with several key requirements of the EU Cyber Resilience Act:

* Secure Software Development: FAIR's decentralized architecture and open governance reduce the risk of unauthorized code changes and supply chain attacks, supporting secure development practices.
* Vulnerability Management: By minimizing central points of failure and enabling transparent updates, FAIR helps site owners respond quickly to vulnerabilities and maintain secure software.
* Data Minimization and Protection: FAIR limits the collection and storage of personal data, reducing the risk and impact of data breaches and supporting the CRA's focus on data protection.
* Transparency and Accountability: FAIR's open processes and clear documentation make it easier for site owners to demonstrate compliance with CRA requirements for transparency and accountability in software supply chains.
* Resilience: Decentralized distribution and reduced reliance on single infrastructure points increase the resilience of the software ecosystem, as required by the CRA.

# Gemara Project Governance

As a developing project, Gemara aims to have a quick development cycle where decisions and community issues are resolved promptly while capturing the input of interested stakeholders.

Gemara has no formal collegiate body in charge of steering. Decisions are guided by the consensus of community members who have achieved maintainer status.

While maintainer consensus shall be the process for decision making, all issues and proposals shall be governed by the project's [Guiding Governance Principles].

## Guiding Governance Principles

Any issues or proposals brought to the project's maintainers shall be framed in the [Guiding Governance Principles].
Proposals not adhering to said principles shall not be considered for consensus.

### Follow Layer-Based Architecture

The six-layer model (Guidance, Controls, Policy, Evaluation, Enforcement, Audit) provides a clear structure for organizing compliance activities. Changes respect this architectural model and relationships between layers.

### Ensure Engineering-Centric Design

Schemas and models must prioritize practical, implementable solutions aligned with how GRC professionals apply engineering practices to compliance work, ensuring relevance and usability.

### Use Schema-Driven Development

Machine-readable schemas (CUE) form the foundation for all compliance activities, ensuring consistency, validation, and automation throughout the GRC lifecycle.

### Incremental and Backward-Compatible

Changes prioritize backward compatibility. Breaking changes are rare and require careful consideration, community input, and clear migration paths.

## Maintainer Consensus

To reach a decision on an issue or proposal, the proponents must seek maintainer consensus.

In the context of this document, "maintainer consensus" means collecting approvals from at least 51% of the current maintainer body, with enough time for all maintainers to review (usually 2 business days), and without a dissenting maintainer opinion.

This document does not prescribe a method of voting. Any mechanism that enables the collection of positive/negative votes associated with an identity may be used. Examples of this include voting through "thumbs up/down" emojis or with "+1" comments in issues.

## Contributor Roles

For a complete description of all roles, requirements, and promotion processes, see the [Contributor Ladder]. Changes to the [Contributor Ladder] require approval from at least 66% of active maintainers.

### Sponsoring Committees

To nominate a community member as a candidate for a role, a group of maintainers may file a nomination. The committee shall meet the following criteria to be qualified to file the nomination:

- The number of members in the committee shall not be less than two (2).
- Whenever the number of organizations with maintainers in the project is more than two (2), committee members shall be from different organizations.

## Revisions to the Governance Model

The governance model is revisited every six months to address community needs. At any point, a GitHub issue may propose changes to governance. Proposals require approval from at least 66% of active maintainers.

## Acknowledgements

This document was adapted from the Security Baseline Governance [documentation](https://github.com/ossf/security-baseline/blob/main/governance/GOVERNANCE.md).

[MAINTAINERS.md]: ./MAINTAINERS.md
[Contributor Ladder]: ./CONTRIBUTOR_LADDER.md
[maintainer consensus]: #maintainer-consensus
[Sponsoring Committee]: #sponsoring-committees
[Guiding Governance Principles]: #guiding-governance-principles
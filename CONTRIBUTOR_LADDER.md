# Contributor Ladder

Everyone is welcome to contribute to Gemara through discussion, issues, and pull requests.

The following roles define additional responsibilities and privileges a community member may receive.  Moving up the ladder is meant to be achievable, not bureaucratic.

All governance decisions follow the processes defined in the [governance] document.

| Role | Responsibilities | Requirements                                                        | Defined by |
|:---|:---|:--------------------------------------------------------------------|:---|
| Member | Active contributor, participates in discussions and reviews | Multiple contributions over time, sponsored by 1 maintainer | GitHub `gemaraproj` Organization Member |
| Approver | Review and approve PRs within a specific scope | Member with history of quality reviews | [CODEOWNERS] entry for specific files or directories |
| Core Maintainer | Org-wide oversight, spec authority, binding governance votes | Approver with cross-project contributions | [MAINTAINERS.md] entry and GitHub `gemara-maintainers` Team |
| Community Manager | Outreach, moderation, documentation maintenance (lateral role) | Active community engagement | [MAINTAINERS.md] entry |

## All New & Established Contributors

Anyone participating in a Gemara meeting, event, or contribution is expected to follow the [OpenSSF Code of Conduct].

New contributors should be welcomed by existing members, helped with PR workflow, and directed to relevant documentation and communication channels.

### Definition of Contributions

Contributions are meaningful engagements that advance the goals of the project. These include, but are not limited to:

- Submission of pull requests that are subsequently merged.
- Participation in discussions on issues, pull requests, or community channels.
- Contribution to design proposals or reviews.
- Documentation improvements.
- Helping others in discussions or community calls.
- Event planning or managing community tools and resources.

## Member

A Member is an active community member who has made repeated, meaningful contributions to the project over time.

**Defined by:** GitHub `gemaraproj` Organization Membership.

### Requirements

- Enabled two-factor authentication on their GitHub account.
- Have made multiple [contributions] to the project, enough to demonstrate an ongoing commitment.
- Sponsored by one (1) existing maintainer (Approver or Core).

### Process

1. A sponsor opens a GitHub issue in the [`gemaraproj/.github`](https://github.com/gemaraproj/.github) repository requesting the contributor be added to the `gemaraproj` GitHub Organization.
   - The issue should summarize the contributor's contributions to date.
2. Any Core Maintainer adds the new Member to the organization.

### Responsibilities & Privileges

- Can have issues and PRs assigned to them.
- Can be invited to review PRs.

## Approver

An Approver reviews and approves contributions from other members within a specific scope. Approval is focused on holistic acceptance of a contribution including backward/forward compatibility, adherence to conventions, and interactions with other parts of the system.

**Defined by:** [CODEOWNERS] entry for specific files or directories.

### Requirements

- Active [Member] for at least three (3) months.
- History of quality reviews and contributions within a specific scope.

Community members may become Approver candidates through:

- Nomination by a [sponsoring committee] at any time.
- Self-nomination after meeting the above requirements.

### Process

1. The nominator opens a pull request to add the candidate to the relevant [CODEOWNERS] file.
   - The PR must remain open for seven (7) days to gather feedback, or until all existing Approvers for that scope have responded, whichever is first.
2. Any current Approver or Maintainer may request changes or object to the nomination.
3. Once approved, the PR is merged.

### Responsibilities & Privileges

- Review and approve PRs within their designated scope.
- Ensure contributions meet the project's conventions and quality standards.
- Adhere to the general responsibilities of a [Member].

## Core Maintainer

A Core Maintainer has organization-wide oversight, maintains the Gemara spec, and holds a binding vote on project [governance] decisions.

**Defined by:** [MAINTAINERS.md] entry and GitHub `gemara-maintainers` Team.

### Requirements

Community members may become maintainer candidates through:

- Nomination by a [sponsoring committee] at any time
- Self-nomination after actively contributing to Gemara monthly for six months or more

Candidates must be an active [Approver] with sustained cross-project contributions. Roles are not mutually exclusive; a [Community Manager] may also hold [Approver] status and progress to Core Maintainer.

### Process

Nominations are submitted via pull request to update Gemara's [MAINTAINERS.md]. After validation, [maintainer consensus] is sought. Upon consensus, the PR is merged and the new maintainer is added to the `gemara-maintainers` GitHub Team.

### Responsibilities & Privileges

Maintainers guide the project's technical direction and make decisions through [maintainer consensus]. Maintainers must uphold the [Guiding Governance Principles] and ensure all proposals align with them.

- Maintainers can review, approve, and merge pull requests.
- Maintainers have access to repository management settings.
- Maintainers have binding votes in [maintainer consensus] decisions.
- Maintainers can form [sponsoring committees] to nominate new maintainers and Community Managers.

### Continued Maintainer Status

Maintainer status requires regular activity and adherence to the [OpenSSF Code of Conduct].

### Emeritus Maintainers

Emeritus maintainers are listed in a separate section on Gemara's [MAINTAINERS.md].
A maintainer may be given Emeritus status after six months of inactivity (e.g., no pull request or issue interactions) or may self-assign Emeritus status via pull request.
A maintainer may return from Emeritus status through [maintainer consensus] and a pull request.

## Community Manager

A Community Manager is a lateral role focused on community engagement, outreach, moderation, and documentation maintenance. It is not part of the technical contributor ladder.

**Defined by:** [MAINTAINERS.md] entry.

### Requirements

Community members may become Community Managers through:
- Nomination by a [sponsoring committee] at any time.
- Self-nomination after actively contributing to Gemara in areas such as moderation, event organization, content creation, and user support.

### Process

Nominations are submitted via pull request to update Gemara's [MAINTAINERS.md] under `Community Managers`. After validation, there must be **unanimous approval** from all active maintainers. Upon consensus, the PR is merged to confirm the new community manager.

Removal of a community manager requires [maintainer consensus] on a corresponding pull request.

### Responsibilities & Privileges

Community Managers manage community engagement and outreach without maintainer responsibilities.

- Community Managers receive access to Gemara community tools (GitHub Pages, social media accounts, etc.).
- Maintain and improve project documentation (website, guides, onboarding materials).
- The nature of the role is neutral facilitator; thus, they **do not** have a binding vote in [maintainer consensus].

## GitHub Team Mapping

The following table maps contributor ladder roles to GitHub Teams and their repository permission levels.

| GitHub Team                              | Role                | Permission | Scope                                                        |
|:-----------------------------------------|:--------------------|:-----------|:-------------------------------------------------------------|
| `@gemaraproj/gemara-<project>-approvers` | [Approver]          | Write      | Specific repositories (review scope defined by [CODEOWNERS]) |
| `@gemaraproj/gemara-maintainers`         | [Core Maintainer]   | Admin      | All repositories                                             |
| `@gemaraproj/gemara-documentation`       | [Community Manager] | Write      | `gemara` (website content only)                              |

[Members][Member] receive Read access as the organization-level base permission. No dedicated team is required.

Team membership changes follow the processes defined for each role above.

## Inactive Members

Maintaining a healthy community requires encouraging active participation. It is natural for people's focus to shift over time, and no one is expected to contribute forever.

An inactive member is anyone holding a role above with **zero** qualifying [contributions] in the preceding six (6) months. Inactive members may:

- Self-assign **Emeritus** status via pull request at any time.
- Be moved to Emeritus after six months of inactivity by any maintainer via pull request.

Emeritus members are listed in a separate section on [MAINTAINERS.md]. An Emeritus member may return to active status through [maintainer consensus] and a pull request.

## Revisions to the Contributor Ladder

Changes to this document require approval from at least 66% of active maintainers, as defined in the [governance] document.

## Acknowledgements

The contributor ladder was inspired by the FINOS Common Cloud Controls [member roles](https://github.com/finos/common-cloud-controls/blob/main/docs/governance/member-roles.md).

[governance]: ./GOVERNANCE.md
[MAINTAINERS.md]: ./MAINTAINERS.md
[CODEOWNERS]: https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-code-owners
[OpenSSF Code of Conduct]: https://openssf.org/community/code-of-conduct/
[maintainer consensus]: ./GOVERNANCE.md#maintainer-consensus
[Guiding Governance Principles]: ./GOVERNANCE.md#guiding-governance-principles
[Sponsoring Committee]: ./GOVERNANCE.md#sponsoring-committees
[contributions]: #definition-of-contributions
[Member]: #member
[Approver]: #approver
[Core Maintainer]: #core-maintainer
[Community Manager]: #community-manager

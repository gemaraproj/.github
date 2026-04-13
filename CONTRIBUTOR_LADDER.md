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
- Appointed by a [Core Maintainer].

### Process

1. An appointer opens a pull request to add the appointee to the relevant [CODEOWNERS] file.
   - The PR must remain open for seven (7) days to gather feedback, or until all existing Approvers for that scope have responded, whichever is first.
2. Any current Approver or Maintainer may request changes or object to the appointment.
3. Once approved, the PR is merged.

### Responsibilities & Privileges

- Review and approve PRs within their designated scope.
- Ensure contributions meet the project's conventions and quality standards.
- Adhere to the general responsibilities of a [Member].

## Core Maintainer

A Core Maintainer has organization-wide oversight, maintains the Gemara spec, and holds a binding vote on project [governance] decisions.

**Defined by:** [MAINTAINERS.md] entry and GitHub `gemara-maintainers` Team.

### Requirements

- Active [Approver] with sustained cross-project contributions.
- Nomination by a [sponsoring committee], or self-nomination.

### Process

1. A nominator opens a pull request to update [MAINTAINERS.md].
2. Approval requires [maintainer consensus].
3. Once approved, the PR is merged and the new maintainer is added to the `gemara-maintainers` GitHub Team.

### Responsibilities & Privileges

- All [Approver] privileges across all repositories.
- Access to organization-level settings and repository management.
- Binding votes in [maintainer consensus] decisions.
- Guide the project's overall technical direction and uphold the [Guiding Governance Principles].
- Form [sponsoring committees] to nominate new Core Maintainers and Community Managers.

## Community Manager

A Community Manager is a lateral role focused on community engagement, outreach, moderation, and documentation maintenance. It is not part of the technical contributor ladder.

**Defined by:** [MAINTAINERS.md] entry.

### Requirements

- Active community engagement in areas such as moderation, event organization, content creation, and user support.
- Nomination by a [sponsoring committee], or self-nomination.

### Process

1. A nominator opens a pull request to update [MAINTAINERS.md].
2. Approval requires **unanimous consent** from all active [Core Maintainers][Core Maintainer].
3. Removal of a Community Manager requires [maintainer consensus] on a corresponding pull request.

### Responsibilities & Privileges

- Access to Gemara community tools (GitHub Pages, social media accounts, etc.).
- Maintain and improve project documentation (website, guides, onboarding materials).
- Neutral facilitator; Community Managers **do not** hold a binding vote in [maintainer consensus].

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

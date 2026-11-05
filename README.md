# Agent Name Service (ANS) Project Governance

This repository holds the governance documents for the Agent Name Service
(ANS) project. It covers every repository in the `agentnameservice` GitHub
organization. It lives at `agentnameservice/governance`.

## Documents

| Document | What it is |
| --- | --- |
| [CHARTER.md](CHARTER.md) | The Technical Charter defines the project, the Technical Steering Committee (TSC), voting, and the IP policy. |
| [GOVERNANCE.md](GOVERNANCE.md) | How the project runs day to day: decisions, proposals, specification and code change rules, SDK maintenance, releases, repositories, meetings, disputes. |
| [CONTRIBUTOR_LADDER.md](CONTRIBUTOR_LADDER.md) | The roles (Contributor, Member, Reviewer, Maintainer, TSC Member, TSC Chair, Vice Chair, Advisor, Emeritus): what they are for, how you get them, how you lose them. |
| [RATIONALE.md](RATIONALE.md) | Why the governance rules are structured this way. An explanatory companion that adds no requirements. |
| [TSC.md](TSC.md) | The TSC roster, officers, portfolios, terms, and election calendar. |
| [MAINTAINERS.md](MAINTAINERS.md) | The index of repository Maintainer teams. |
| [CONTRIBUTING.md](CONTRIBUTING.md) | The org-wide contribution guide: DCO, pull request flow, review rules, AI disclosure. Each repository links here. |
| [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) | The Code of Conduct and its reporting, investigation, and enforcement procedures. |
| [SECURITY.md](SECURITY.md) | How to report vulnerabilities and how the project responds. |
| [DCO](DCO) | Developer Certificate of Origin 1.1, verbatim. |
| [decisions/](decisions/) | Numbered record of TSC decisions. |
| [templates/](templates/) | Proposal sections for a PR that serves as a proposal, and the decision record template. |

`templates/` contains Markdown templates. Shared GitHub issue forms and
workflow implementations are maintained separately from these documents.

Who may change each document is in GOVERNANCE.md Section 14.

## How the pieces fit together

The Charter is short and mostly boilerplate on purpose. It says what the
project is, that a TSC runs it, and what licenses apply. It then hands
everything operational to documents the TSC controls on its own. That is how
LF projects are normally set up: the Charter needs LF approval to change, so
anything that might need to change more than once a year lives in
GOVERNANCE.md and CONTRIBUTOR_LADDER.md instead.

```
CHARTER.md            legal foundation, changes rarely
  |- GOVERNANCE.md     how decisions get made, how repos are run
  |- CONTRIBUTOR_LADDER.md   who can do what, and how they got there
  |- TSC.md             TSC membership, officers, and terms
  |- MAINTAINERS.md      repository teams and local arrangements
  |- CONTRIBUTING.md / CODE_OF_CONDUCT.md / SECURITY.md   what every repo points at
```

## Relationship to the code repositories

Each repository in the organization keeps a short `CONTRIBUTING.md`,
`CODE_OF_CONDUCT.md`, and `SECURITY.md` that point here, plus its own
`MAINTAINERS.md` and `CODEOWNERS`. The org-level `.github` repository carries
the shared defaults for repositories that do not override them.

## License

The documents in this repository are licensed under
[CC BY 4.0](LICENSE). Code and specification licenses are set by
[CHARTER.md](CHARTER.md) Section 7.

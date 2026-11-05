# Maintainers

This is the index of which team maintains each repository. Current team
membership and GitHub access are recorded in
[the organization team configuration](https://github.com/agentnameservice/.github/blob/main/peribolos.yml).
Each repository's `MAINTAINERS.md` links to its team and records local quiet
periods or interim appointments. `CODEOWNERS` routes reviews to those teams.

Roles are defined in [CONTRIBUTOR_LADDER.md](CONTRIBUTOR_LADDER.md). SDK
maintenance is covered by Section 8 of [GOVERNANCE.md](GOVERNANCE.md).

## Repositories

The Team column identifies the repository's merge team. TSC voting appointments
remain recorded in [TSC.md](TSC.md); TSC fallback review access does not change
which team maintains a project repository.

| Repository | Role in the project | Team |
| --- | --- | --- |
| `ans-spec` | Specifications, schemas, conformance vectors | `@agentnameservice/spec-maintainers` |
| `ans` | Reference implementation (RA, TL, verifier, dev DNS) | `@agentnameservice/ans-maintainers` |
| `ans-sdk-go` | Go SDK and CLI | `@agentnameservice/sdk-go-maintainers` |
| `ans-sdk-rust` | Rust SDK | `@agentnameservice/sdk-rust-maintainers` |
| `ans-sdk-java` | Java SDK | `@agentnameservice/sdk-java-maintainers` |
| `agent-trust-discovery` | Trust index | `@agentnameservice/trust-maintainers` |
| `trust-index-spec` | Trust index specification | `@agentnameservice/trust-index-spec-maintainers` |
| `ans-openshell` | ANS OpenShell integration | `@agentnameservice/ans-openshell-maintainers` |
| `ans-gateway-auth` | ANS gateway authentication | `@agentnameservice/ans-gateway-auth-maintainers` |
| `homebrew-ans`, `scoop-ans` | CLI distribution taps | `@agentnameservice/sdk-go-maintainers` |
| `.github` | Org defaults | `@agentnameservice/tsc-owners` |
| `governance` | This repository | `@agentnameservice/tsc` |

## Hosted test environments

| Environment | Hosted by | Contact | Notes |
| --- | --- | --- | --- |
| [none yet] | | | |

## Quiet periods

Project-wide dates when the review reply expectation is suspended
(GOVERNANCE.md Section 7). Repository-specific ones go in that repository's
`MAINTAINERS.md`.

| From | To | Note |
| --- | --- | --- |
| | | |

## Emeritus

| Name | GitHub | Former role | Repository | Until |
| --- | --- | --- | --- | --- |
| | | | | |

## Template

The template for a repository's own `MAINTAINERS.md` is
[templates/MAINTAINERS.md](templates/MAINTAINERS.md).

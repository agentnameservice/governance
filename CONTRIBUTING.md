# Contributing to ANS

Thanks for your interest in the Agent Name Service (ANS) project. This guide
applies to every repository in the `agentnameservice` organization. Build and
test instructions for a specific repository are in that repository's README.

## Before you start

- Read the [Code of Conduct](CODE_OF_CONDUCT.md). It applies everywhere the
  project talks.
- **Do not report security problems in a public issue.** See
  [SECURITY.md](SECURITY.md).
- Open an issue before a pull request unless the change is tiny. Issues are
  where triage and prioritization happen, and every pull request needs one to
  link to.

## Ways to contribute

Code and specification text are not the only contributions. Answering
questions, triaging issues, reviewing pull requests, writing examples, and
testing an SDK against the specification all count, including toward the
roles in the [Contributor Ladder](CONTRIBUTOR_LADDER.md).

## The pull request flow

1. Fork the repository and create a branch from `main`.
2. Make your change. Add or update tests. For specification changes, update
   the machine-readable artifacts (schemas, OpenAPI, conformance vectors) in
   the same pull request.
3. Sign off every commit (`git commit -s`). See DCO below.
4. Use a Conventional Commits title: `feat:`, `fix:`, `docs:`, `spec:`,
   `test:`, `chore:`. Releases are generated from these.
5. Open the pull request. In the description say what changed and why, link
   the issue with a closing keyword (`Fixes #123`), and for specification
   changes say whether it is **editorial** or **normative** (Section 6.1 of
   [GOVERNANCE.md](GOVERNANCE.md)).
6. Respond to review. The author is responsible for making the follow-up
   changes.

What a change needs before it can merge is in Sections 6 and 7 of
[GOVERNANCE.md](GOVERNANCE.md): one approval for most changes, two for the
sensitive categories listed there. A Maintainer who is not the author does
the merge, and you never approve your own change. Some changes need an
accepted proposal first; Section 5 lists them.

## Developer Certificate of Origin

The project uses the Linux Foundation contribution model. Every commit must
carry a `Signed-off-by:` trailer certifying the
[Developer Certificate of Origin](DCO), which is your statement that you have
the right to submit the change under the project's license. Sign off with:

```
git commit -s
```

Missing sign-offs on an existing branch can be fixed with
`git rebase --signoff origin/main` followed by a force push. The org-wide
[DCO app](https://github.com/apps/dco) checks every pull request. Bot-authored
commits (Dependabot, release-please) and merge commits are exempt.

Sign off with your real name and a working email address. Sign-offs from
automated tools are not accepted.

## AI-assisted contributions

AI-assisted contributions are welcome **with disclosure**, following the
[Linux kernel convention](https://docs.kernel.org/process/coding-assistants.html):

- Say which tool and model you used in the pull request's **AI assistance**
  section, for example `Assisted-by: Claude Code (claude-fable-5-1)`.
- AI tools must never add `Signed-off-by:` lines. The DCO certification
  belongs to the human submitter, who is responsible for the correctness and
  licensing of the contribution.

## Licensing your contribution

Contributions follow Section 7 of the [Charter](CHARTER.md): new inbound
code, including schemas, OpenAPI documents, and conformance test vectors,
uses Apache 2.0; new specifications and other documentation use CC BY 4.0;
data uses CDLA-Permissive 2.0. Outbound code uses Apache 2.0, except that
pre-existing or third-party code may remain available under its applicable
license. Alternative licenses require a TSC exception under Charter 7.c.
Put an SPDX identifier at the top of new files. Contributors retain copyright
in their contributions.

## Review expectations

The repository's Reviewers and Maintainers aim to give you a first reply
within 10 days, outside any quiet period listed in its `MAINTAINERS.md`.
That is a reply, not an approval; a full review takes as long as it takes.
Reviews use GitHub's review states: "Request changes" blocks, "Comment" does
not, "Approve" approves. When you have addressed requested changes, push and
click **Re-request review** on that reviewer. That is what notifies them; a
comment or @-mention may be missed. If nothing has happened 20 days after a
re-request, say so on the pull request and mention any TSC member.

If it is your turn (changes requested or checks failing) and nothing happens
for 60 days, a bot will ask whether you are still working on it and add a
`stale` label. Thirty days after that the pull request is closed. Reopen it
any time by pushing or asking; the issue stays open. A pull request waiting on
reviewers is never closed for inactivity.

To help reviews go faster: keep pull requests small, review other people's
pull requests, and split unrelated changes.

## Proposing something bigger

New specification documents and profiles, conformance changes, breaking
wire or API changes, and repository or governance changes start with a
proposal. Open one with the Proposal issue form in the affected repository,
or, if a pull request will serve as the proposal, put the sections from
[templates/proposal.md](templates/proposal.md) in its description. Section 5
of [GOVERNANCE.md](GOVERNANCE.md) explains the process.

## Getting more involved

The [Contributor Ladder](CONTRIBUTOR_LADDER.md) explains how to become a
Member, Reviewer, or Maintainer, and what each role expects of you.

# Why the rules are shaped this way

> **Non-normative rationale.** See [README.md](README.md).

Projects that move from one company into a foundation tend to fail in the
same handful of ways. This page lists those pitfalls and what these documents
do about each one, so a reader can see the intent behind a rule before
arguing with it. Nothing here is normative; the linked documents are.

## The founding company keeps control in practice

The most common outcome: a neutral-looking foundation project where one
employer still holds every seat and every merge button.

- The Charter limits each organization and its affiliates to fewer than
  half of the seated TSC after startup or the first TSC election, whichever
  comes first (Charter 2.d).
- If an election cannot seat at least five members within that cap,
  incumbents can hold over until a by-election. While the TSC exceeds the
  cap, the specified votes also need support from outside the largest
  organization (Charter 2.d).
- The TSC grows from five to nine over the first two elections, so widening
  participation is scheduled rather than left to the incumbents (GOVERNANCE
  3.1). New seats with no eligible candidate stay vacant and never count
  toward a threshold.
- Regular TSC elections give active Members, Reviewers, Maintainers, and
  sitting TSC members a vote. Startup and vacancy appointments provide
  continuity (GOVERNANCE 3.2).
- Normative specification changes need an approver from a different
  organization than the author when the roster allows (GOVERNANCE 6.2).
- Roles belong to people, not employers. Changing jobs changes nothing except
  the TSC cap (Ladder, rules).

## Seats filled by name, not by work

Author lists and courtesy appointments produce TSC members who never read
what they vote on, and whose absence blocks votes that need a majority of all
members.

- From the first TSC election on, every candidate, incumbent or not, must
  be a Maintainer or Reviewer (GOVERNANCE 3.2). A seat is not a qualification
  to keep it.
- The initial TSC can choose its first Chair and Vice Chair from all its
  seated members. The Maintainer waiver covers only those initial elections
  and terms; later officer elections require a Maintainer (GOVERNANCE 3.3).
- People whose input is wanted without a vote become Advisors (GOVERNANCE 3.5).
- A member who misses three consecutive votes or leaves TSC requests
  unanswered for 90 days can be replaced after contact and a vote
  (GOVERNANCE 3.4). A quiet quarter counts against nobody.

## Governance welded into the legal document

If review rules live in the Charter, changing a review rule needs a
two-thirds vote and Linux Foundation approval, so nobody changes it.

- The Charter sets the mission, TSC authority, and licenses. Day-to-day
  procedures live in GOVERNANCE.md and the Ladder (Charter 2.e and 2.g).
- Most changes to those documents need a TSC majority after a 14-day
  proposal. Protected provisions need two-thirds, and during startup a vote
  from outside the largest organization (GOVERNANCE 14).

## Nobody owns the administration

Foundation requests go unanswered, GitHub permissions drift, inactive people
keep access, and the project looks dead from outside while work continues.

- A Chair with listed duties and a ten-business-day reply target to LF
  (GOVERNANCE 3.3), a Vice Chair who steps in when the Chair does not, and
  portfolios so the work is spread (GOVERNANCE 3.6).
- An annual access review (GOVERNANCE 9.3) and a quarterly health check that
  brings repository activity, review delays, and maintenance capacity to the
  TSC's attention (GOVERNANCE 9.4).

## The specification and the implementations drift apart

A specification that changes faster than anyone implements it stops being a
specification.

- A normative change in `ans-spec` opens tracking issues in the
  reference implementation and each maintained SDK before merge. A
  specification release needs the implementation work completed and
  conformance CI passing, or an explicit deferral (GOVERNANCE 6.2, 6.3).
- Schemas, OpenAPI, and conformance vectors are code, change in the same pull
  request as the text, and are versioned with the specification (Charter
  7.b.iv, GOVERNANCE 6.2).

## Process built for fifty people applied to five

Heavy proposal processes on a small team mean nothing gets done or the
process gets ignored, which teaches everyone that the documents do not
matter.

- Ordinary normative changes need two approvals. Proposals are reserved
  for the higher-impact changes listed in GOVERNANCE 5, such as new profiles,
  breaking released interfaces, and governance changes.
- Lazy consensus handles routine process decisions. Code and specification
  changes need explicit approvals; questions with a voting threshold need a
  vote (GOVERNANCE 4).
- A pull request can be the proposal. There are no standing meetings
  (GOVERNANCE 5, 11).
- TSC members can extend project-wide windows once by asking; Maintainers
  can do the same for their repository's windows (GOVERNANCE 4.4).

## Review expectations that ignore real lives

A response deadline written for a company team punishes volunteers, and a
missed one becomes a reason to leave.

- The ten-day target is for a first reply, not an approval, and applies to a
  repository's reviewers as a group. People marked away are excluded.
  Repositories and the project can declare quiet periods. Missing it triggers
  escalation, never a penalty (GOVERNANCE 7).
- If a repository lacks reviewers, a TSC member or another repository's
  Maintainer may supply the missing approval (GOVERNANCE 7). The TSC team has
  Write access and code-owner eligibility so that fallback works in GitHub,
  while merging stays with the repository's Maintainers. The reason for using
  the fallback is recorded in the pull request.

## Pull requests that die of neglect

Contributors cannot tell whether anyone saw their work, and old pull requests
pile up until the queue is meaningless.

- Blocking feedback is a "Request changes" review, never a bare comment.
  Authors re-request review to hand it back, so the page always shows whose
  turn it is (GOVERNANCE 7.1).
- The inactivity rule gives authors a reminder before closing long-idle
  pull requests. One waiting on reviewers stays open (GOVERNANCE 7.2).

## Licensing surprises after the donation

Finding out post-donation that the code was under a different license than
the Charter says, or that implementers have no patent grant for the
specification, is expensive to unwind.

- New inbound code uses Apache 2.0. Outbound code also uses Apache 2.0,
  except that pre-existing or third-party code may remain available under its
  applicable license (Charter 7.b.i, 7.b.iii).
- New specifications use CC BY 4.0. CC BY does not grant implementers a patent
  license (Charter 7.b.v).
- A DCO sign-off records the contributor's certification that they have the
  right to submit their work. CONTRIBUTING.md sets the sign-off requirements
  and exemptions.

## No way in for outside contributors

Projects that only have "maintainer" and "everyone else" never grow past the
founding team.

- Member and Reviewer are deliberately low bars with clear criteria and a
  sponsor (Ladder). Membership is offered at donation to everyone who already
  meets them.
- Emeritus lets people leave and come back without starting over (Ladder).

## Security handled by whoever notices

- One security policy for every repository, private reporting as the primary
  channel, published timelines, embargo coordination for specification flaws,
  and a Security portfolio with clear responsibilities (SECURITY.md,
  GOVERNANCE 3.6).

## Decisions that only exist in someone's memory

- Every TSC decision gets a record in `decisions/` that links to the
  discussion. Meetings are open by default; closed sessions are limited to
  specified conduct and appeal matters, embargoed security reports, legal
  advice, or personal data. Attendance and outcomes are still recorded
  publicly (GOVERNANCE 4.3, 11).

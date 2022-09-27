# Governance

Coraza is an open-source WAF solution compatible with seclang and CoreRuleset.

The Coraza project aims for open and transparent governance and decision-making, thus encouraging community building and contribution.

A formal governance structure helps us to

- Provide a structure for individuals to become involved in the project.
- Communicate all processes for members to operate within the project.
- Document a system for open product development, roadmapping, and planning.
- Provide a means for making decisions if consensus cannot be reached.

This document describes the rules and governance of the Coraza project. It is meant to be followed by all the developers of the project and the Coraza community.

## Community overview

On a high level, the key moving parts of the community are:

- **GitHub activity** (issues + pull requests)
- **Slack community**
  - [`#coraza`](https://owasp.slack.com/archives/C02BXH135AT) channel is where all the discussions and questions happen in the coraza community
  - [`#coraza-core`](https://owasp.slack.com/archives/C034AF28KPV) channel is where internal discussions around the team happen.
- **Monthly meetings** (last wednesday of every month) to give an update on the open topics in coraza and held votings for new team members. It's being held in the `#coraza` channel.

## Values

Coraza community strives for trust, respect, kindness, giving feedback effectively, and building a welcoming environment. The Coraza developers generally decide by consensus.

## Projects

Each project must have a `CODEOWNERS` file with at least one code owner. Where a project has a release process, access and documentation should be such that more than one person can perform a release. Releases should be announced on the `#coraza` channel. Any new projects should be first proposed on the `#coraza-core` channel following the voting procedures listed below.

## Decision making

Coraza is a meritocratic, consensus-based community project.

### Team members

Team member status may be given to those who have made ongoing contributions to the Coraza project for at least 2 months. This is usually in the form of significant code improvements and/or notable work on documentation.

New members may be proposed by any existing member in the monthly meeting. It is highly desirable to reach consensus about acceptance of a new member. However, the proposal is ultimately voted on by a formal [majority vote](#majority-vote).

If the new member proposal is accepted, the proposed team member will be pinged in a github issue on this repository and confirm its acceptance.

Team members may retire at any time by opening a github issue in this repository requesting for removal.

Team members can be removed by [majority vote](#majority-vote) opening a github issue and voting in the next 48 hours.
For this vote, the member in question is not eligible to vote and does not count towards the quorum.
Any removal vote can cover only one single person.

In case a member leaves, the [offboarding](#offboarding) procedure is applied.

The current team members can be found under this link.

### Code owners

Code owners lead one or more project(s) or parts thereof and serve as a point of conflict resolution amongst the contributors to this project. Ideally, code owners are also team members, but exceptions are possible for suitable code owners that, for whatever reason, are not yet team members.

Changes in code ownership have to be announced in the `#coraza-core` channel. They are decided by [rough consensus](#consensus) and formalized by changing the `CODEOWNERS` file of the respective repository in a PR.

Code owners are granted commit rights to all projects covered by this governance.

A code owner or committer may resign by notifying the team. A code owner with no project activity for a year is considered to have resigned. Code owners that wish to resign are encouraged to propose another team member to take over the project. A project with no code owners might be considered to be archived.

A project may have multiple code owners, as long as the responsibilities are clearly agreed upon between them. This includes coordinating who handles which issues and pull requests.

### Administrators

Administrators are team member with access to manage the [Coraza organization](https://github.com/corazawaf). Any change in the organization should be agree upon vote in the `#coraza-core` channel. The role of administrator does not represent any kind of hierarchy among team members.

For the sake of independence, no two administrators can work for the same company despite the regime (full time, consultancy, etc).

### Technical decisions

Technical decisions that only affect a single project are made informally by the code owners of this project, and [rough consensus](#consensus) is assumed. Technical decisions that span multiple parts of the Coraza project should be discussed and made on an adhoc github issue.

Decisions are usually made by [rough consensus](#consensus). If no consensus can be reached, the matter may be resolved by [majority vote](#majority-vote).

## Changes to Governance

We believe governance needs to adapt in order to be effective long term. This governance document itself can be extended or modified as our community and project grows and our needs change.

A change in our governance structure should be a rare occurrence and should face sufficient scrutiny and review. To this end, the rules that apply to modifications to the Feast Governance structure are more stringent:

- Governance changes are made through PRs to the [corazawaf/community](https://github.com/corazawaf/community) repository.
- Rough consensus applies to governance changes, but the proposed changes must be public for at least 7 days instead of 48 hours before they are accepted.
- If there is opposition to a change, a vote will be held by team members.
- Voting is asynchronous. All team members must be notified of a vote through the github issue.
- Team members must be given at least 7 days to respond.
- Voting requires a [majority vote](#majority-vote) in order to pass a decision.
- A quorum is required for voting. A quorum is 60% of code owners.

### Other matters

Any matter that needs a decision may be called to a vote by any member if they deem it necessary. For private or personnel matters, discussion and voting takes place on the  `#coraza-core` channel.

## Voting

The Coraza project usually runs by informal consensus, however sometimes a formal decision must be made.

Depending on the subject matter, as laid out [above](#decision-making), different methods of voting are used.

For all votes, voting must be open for at least three workdays. The end date should be clearly stated in the call to vote. A vote may be called and closed early if enough votes have come in one way so that further votes cannot change the final decision.

In all cases, all and only [team members](#team-members) are eligible to vote, with the sole exception of the forced removal of a team member, in which said member is not eligible to vote.

Discussion and votes on personnel matters (including but not limited to team membership and code ownership) are held in private on the `#coraza-core` channel. All other discussion and votes are held in public on the `#coraza` channel.

For public discussions, anyone interested is encouraged to participate. Formal power to object or vote is limited to [team members](#team-members).

### Consensus

The default decision making mechanism for the Coraza project is rough consensus. This means that any decision on technical issues is considered supported by the team as long as nobody objects or the objection has been considered but not necessarily accommodated.

Silence on any consensus decision is implicit agreement and equivalent to explicit agreement. Explicit agreement may be stated at will.

Consensus decisions can never override or go against the spirit of an earlier explicit vote.

If any [team member](#team-members) raises objections, the team members work together towards a solution that all involved can accept. This solution is again subject to rough consensus.

In case no consensus can be found, but a decision one way or the other must be made, any [team member](#team-members) may call a formal [majority vote](#majority-vote).

### Majority vote

Majority votes must be called explicitly in a separate github issue. The title must be prefixed with `[VOTE]`. In the body, the call to vote must state the proposal being voted on. It should reference any discussion leading up to this point.

Votes may take the form of a single proposal, with the option to vote yes or no, or the form of multiple alternatives.

A vote on a single proposal is considered successful if more vote in favor than against.

If there are multiple alternatives, members may vote for one or more alternatives, or vote “no” to object to all alternatives. It is not possible to cast an “abstain” vote. A vote on multiple alternatives is considered decided in favor of one alternative if it has received the most votes in favor, and a vote from more than half of those voting. Should no alternative reach this quorum, another vote on a reduced number of options may be called separately.

## On- / Offboarding

### Onboarding

The new member is

- added to the list of [team members](link). Ideally by sending a PR of their own, at least approving said PR.
- added to the projects with commit rights.

### Offboarding

The ex-member is

- removed from the list of [team members](link).
- removed from the projects. Optionally, they can retain code ownership of one or more repositories if the [team](#team-members) agrees.
- not allowed to call themselves an active team member any more, nor allowed to imply this to be the case.

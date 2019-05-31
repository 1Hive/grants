# Aragon Nest Proposal: 1Hive PROJECT_NAME_TBD

<br>

## Abstract

> _Description of the problem or a product that could help benefit the ecosystem_

At 1Hive we have been researching and building DAO models for sustainable community driven development of the open source commons. This is no easy task, but we feel like the time has come to make it happen. Our first project is the PROJECT_NAME_TBD suite: an Aragon DAO that combines 5 novel Aragon apps to create a model that is greater than the sum of it's parts.

While this is very exciting, it's only the tip of the iceberg. Most open source software projects want to innovate at the bleeding edge of whatever cool thing they're building. They don't, however, want to reinvent the wheel on governance and fundraising. With this in mind, we are creating the PROJECT_NAME_TBD: a DAO template that will help the open commons thrive.

This will allow open source developers to easily make governance decisions, engage and reward contributors, and provide ongoing sustainable support for their projects. Everything an open source project needs that isn't directly related to the building project itself. This means more time building and less time spent doing everything else. It also means less drama, more engaged users, and sustainable token models to maintain and grow the project.


### Notes from the meeting that have yet to be turned into stuff

A package to create an Aragon DAO with the same basic mechanisms that are employed in molochdao. I think this makes an interesting grant proposal, because it does a few things for us and for the wider Aragon ecosystem.
- Shows the power of the Aragon framework to tackle a specific use case that appears to be top of mind within the Aragon ecosystem. I'm not sure how truthful the statement was, but Ameen said that he tried to figure out how to build Moloch on Aragon and couldn't figure it out. So this project would directly address that criticism.
- Shows the value of the composability and modularity of Aragon Apps (we are not implementing voting, vault, finance, or token manager, they just are installed.)
- The specific components are actually useful by themselves for other DAO use cases. Redemptions is tremendously useful for just about any DAO that may have some sort of liquid treasury (like us). Token Request app provides a simple fundraising option for organizations that resembles raising capital by issuing equity also extremely useful for a broad range of daos (this has been one of the most requested features for a long time). The deposits forwarder could be added to something like the CFDAO as relatively simple spam prevention device. The dissent app, likely only makes sense coupled with redemptions and voting, but still has broader applications when incorporated a more complex DAO than moloch. The delay forwarder is broadly useful, it can be used with voting to ensure that people have the opportunity to exit after the vote outcome is determined but before the action is executed, or directly to allow users to take unilateral action subject to a wait period.
- All of the apps (as far as I can tell) seem to be very simple to implement, meaning that they would probably be good for developers who haven't built an Aragon app before to try and tackle with the help of a more experience member.
- The capability of this grants dao is actually significantly greater than what is currently possible with moloch because it can be extended with thinks like dot voting or pando. The tradeoff between the two would be that moloch is "less code, therefore simpler, and easier to audit" but less flexible and extendable because extensions require forking and writing code rather than installing and configuring apps.

From the 1hive perspective, a "grants" dao template could be used by open source communities to more effectively solicit contributions for a project/ecosystem because the capital contributors have a guaranteed exit. It would likely draw lots of attention to our community, and likely attract more contributors, both of which will be beneficial to our longer term goals (eg HCL, Apiary, onboarding open source communities). And it would bring in capital to the org while allowing us to test and validate our model on real projects.

<br>

## Deliverables

> _List of items that **must** be delivered in order for this problem to be solved_

We are creating the PROJECT_NAME_TBD for 1Hive, the Aragon community, and the open source community as a whole. Concretely this looks like:

Aragon Apps
- Redemptions
- Token Request
- Deposits 
- Dissent Forwarder
- Delay Forwarder

Project Demo
- live DAO demo
- CLI/web deployment template
- developer hub with docs and user guides

Combining these components in a cohesive package will allow open source projects to empower their communities with Aragon DAOs. Imagine if every open source project could be sustainably funded and governed by a decentralized community. We're building the tools to make that possible.

<br>

## Grant size

Funding:
> _Description of the amount and how the funding would be provided to the grantee_
> **Up to $150,000 in DAI, split into chunks paid out over achieved deliverables.**

Success reward:
> _Possible incentive rewards for successful completion of the project delivering all the Deliverables on time_
> **Up to 30,000 ANT, given out when all deliverables are ready.**

Funding: 150k DAI
- $25k for each Aragon App
- $25k for the DAO demo, deployment template, and developer hub

Success Reward:
- $30k ANT

<br>

## Application requirements
> _List of the items required to be showed in a possible application for this grant_

<br>

## Development timeline
> _Description of the timeline in which the deliverables should be developed and delivered_

~ 1 month for each app?
- design draft
- code draft
- bug fixes
- security audit (we're doing these right?)

4-5 months total?
- some apps will go faster than others, and we can work on the deployment template, dev hub, and docs while we build the apps

<br>




# Aragon Nest Proposal: Dandelion Orgs 🌼 <img align="right" src="https://github.com/1Hive/website/blob/master/website/static/img/bee.png" height="80px" />

<br>

## Abstract



[1Hive](https://1hive.org) is interested in exploring how smart organizations (DAOs) can help open source communities better reward and attract contributors. We believe Aragon is the best platform to build on because of the rich ecosystem of existing applications available to Aragon smart organization.

However, we have been disappointed to see promising projects like [Moloch](https://molochdao.com) choose to build a smart organization from scratch rather than extend the Aragon platform. This decision may have been motivated by a desire to minimize code footprint, or due to a lack of understanding of the aragonOS framework. Whatever the reason, we believe that the specific mechanisms can be built for Aragon, and **making these mechanisms modular and composable results in greater overall value**.

We propose breaking the monolithic Moloch concept into the following modular Aragon apps:

- **Redemptions**: Allows users to manage a list of eligible assets held within an organizations `Vault` and allow members of the organization to redeem (burn) organization token in exchange for a proportional amount of the eligible assets.
- **Token Request**: Allows users to propose minting tokens in exchange for a payment to the organization, subject to the approval of existing members.
- **Lock**: Allows an organization to require users to lock a configure amount of tokens for a configurable amount of time in order to forward an intent.
- **Delay**: Allows an organization to require a configurable delay before an action may be executed.
- **Dissent Oracle**: Enhances the voting app to implement an [ACL Oracle](https://hack.aragon.org/docs/acl_IACLOracle) which allows an organization to configure permissions that restrict actions to only members which have recently voted `Yes`.  

These applications can be combined with the existing `Vault`, `Finance`, and `Token Manager` apps to create an organization template based on the fundamental mechanism and game theory used in Moloch. But unlike Moloch, this organization could easily be extended by incorporating the task management and issue prioritization capability of Autark's `Projects` and `Dot Voting` apps or implement streaming payments via Aragon One's upcoming `Payroll` app. We call this variation on the Moloch concept, **Dandelion Orgs**, as they can quickly grow by adding members and capital, but in the event of a contentious decision disperse just as rapidly.

Besides being useful as a template, the individual applications can complement other organization patterns as individual components:

- The CFDAO has a [known vulnerability](https://forum.aragon.org/t/agp-discussion-community-funding-dao/418/21) to spam attacks, and the `Lock` app could be a drop-in solution that would significantly increase the cost of such an attack.
- The `Delay` app could be used to implement optimistic operations within an organization, where members can take actions without requiring a vote, but they can be paused by other members, and canceled via a vote. The delay app would also adopt the same interfaces as the voting app so that it will be compatible with `Proposal Agreements`.
- The `Token Request` application can be used to provide permissioned fundraising capabilities.
- The `Redemptions` app establishes "exit rights" and enables organization's tokens to have a clear baseline valuation based on a claim on the organizations underlying liquid assets.
- The `Dissent Oracle` could provide better voting incentives particularly when combined with an application like `Redemptions` or Aragon Black's upcoming `Fundraising` application which guarantee some sort of exit.   

Beyond simply extending the library of Aragon apps, this proposal intends to highlight the **value** and **network effect** associated with a modular and composable platform like Aragon.

From the 1hive perspective, we have been eager to get started and have gone ahead and implemented the [Redemptions](https://github.com/1Hive/redemptions-app) application and deployed to Rinkeby. If you'd like to try it out you can do so in our Rinkeby [demo org](https://rinkeby.aragon.org/#/tryredemptions/0x18a9713625256548670ad979d51a6b9fad5b6c45). We've also completed some basic feasibility research and have documented how we intend to implement the remaining apps. { [Token Request](https://github.com/1Hive/token-request-app), [Lock](https://github.com/1Hive/lock-app), [Dissent Oracle](https://github.com/1Hive/dissent-voting-app), [Delay](https://github.com/1Hive/delay-app) }

<br>

## Deliverables

> _List of items that **must** be delivered in order for this problem to be solved_

**Aragon Apps**
- Redemptions
- Token Request
- Lock
- Dissent Oracle
- Delay

**Organization Templates**
- Dandelion Org Template

**Documentation**
- Each application will include documentation on how the organization can be deployed, and how to interact with it.

<br>

## Grant size

Funding: 100k DAI
- $15k for each Aragon App (Main-net)
- $10k for Dandelion Org template and onboarding site (Main-net)
- $15k budget for audits and bug bounties

Success Reward:
- $30k ANT

<br>

## Application requirements
> _List of the items required to be showed in a possible application for this grant_

<br>

## Development timeline
> _Description of the timeline in which the deliverables should be developed and delivered_

We estimate needing approximate 1 month to deliver each App, though we plan to do some development in parallel, and conduct audits all at once. We expect to be able to deliver everything to main-net in approximately 5 months. 

<br>

# chaos-engine
Chaos Engine is a App the provides testing scenarios for you to verify that your stack is ready for production.

## Purpose of Chaos-Engine
As a Platform Engineer or operator, I want to be able to validate that my system is robust, and will not crumble under a variety of failures, so that I can be sure that my system is setup in a robust way that is highly available and can withdstand failure. This enables me to scale my business faster without paying the cost of outages.

As a operator, I want to be able to get insights into common failure modes, so that I can have confidence that I have processes in place to handle the failures in a low downtime manner.

As a operator, I need to be able to showcase to my boss that my system is robust against a variety of failure modes, so that he can have confidence that the business being built on top of this stack will be stable as we grow.

As an operator, I may be transitioning to a new technology and therefore need expertise on how to harden my system, so it would be awesome to have database of common failure modes to prepare for, so I know when I have successfully hardened my setup.

## Business Cost of an Outage
Today, tech business lose loads of revenue when an outage happens, and all of our tooling is responsive. We don't really focus on how do we share knowledge about common outage scenarios in a way that allows us to test if we are ready ahead of time. Instead, we hit these issues, use monitoring tools to identify and resolve, and continue prodding forward. There is a huge overlap in the types of outages we all hit, and as the tech industry matures, the types of outages will only overlap more and more across stacks. This means that collecting a centralized data store of outage scnearios, or things to harden would be very useful in minimizing potential outages that might happen. This presents the opportunity to make something far more preventetive in nature, a vaccine if you will against outages.

## How will this work?

What are the pieces of this product puzzle?
1. A clean SDK for writing scenarios.
2. A way to publish scenarios into a publically accessible storage set.
3. A way to run a scenario, monitor the system, and debug it.
4. A way to track and score fixing the scenario. A rating for how well someone responded to a scenario.
5. Ability to extract a scenario's generalizable template, and be able to apply it to your own custom stack, so that you can verify your own ability to withstand that scenario.
6. Ability to run a "report" against your own stack that tells you which scenarios yield an "outage".

## Projects

- [ ] Design Document for how to write a Scenario.
- [ ] Design Document for how to publish, store, update, and retrieve scenarios.
- [ ] UX for how someone can browse scenarios, their scores, etc.
- [ ] Design Document for the running a scenario, and single round of the game.
- [ ] Design Document for Extending Scenarios beyond the playground.
- [ ] Design Document for Running Reports.


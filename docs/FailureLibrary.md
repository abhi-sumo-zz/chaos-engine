# The Failure Library

Features this Library has:
1) 

## Systems Under Duress
1. TravelLogic
2. Demo-App
3. Multi-cloud.

## User Flow
1. User goes to a website, where he/she has the ability to select a scenario and a system to put under duress. The User can select from a set of systems to put under duress and a set of scenarios.

2. After selecting a scenario and the system, the website starts running the scenario in a sandbox kubernetes cluster.

2a. Provisioning agent that starts up the cluster and the system along with the monitoring tools

2b. On user input, we start the failure scenario.

2c. We provide the user with the KubeConfig to connect to the cluster.

2d. We provide a sumo account as the M&T tool to use. (Use the Sumologic API)

2e. User gets access to the Sumo Logic SLA Dashboard for the scenario, and is told that he/she needs to figure out how to fix the SLA violation.
- There needs to logs displayed to the user that tells the user about the state of the scenario (i.e is it starting, how much time has passed, what sla is in violation, etc) Basically a panel in a Sumo Dashboard as a v0.
- Two modes: Challenge & Learn -> In Challenge mode the title should not give away the root cause, and should not let the user get the root cause. In the learn mode, the title and root cause should always be available.
- Reason why: Learn mode is more about understanding and quickly driving action on their own systems, whereas challenge mode is more for training and puzzle solving.

**Challenge mode only for Illuminate**

3. The user starts using the shell to debug the cluster. The timer and monitoring system continues until the SLA is repaired.

4. When the SLA is repaired, the user receives a message that the scenario is over, and is redirected to the webpage where they can see a replay of their debugging process, and a score of how well they did.

## Seeding the Library
1) All Kubernetes post-mortems can be converted to a scenario.
2) The Failure Stories blog posts can be conveted to scenarios.

## For Illuminate
- We will have a leaderboard that will be hooked up to the badge scanner so that we can get the real names.
- A good plushy prize for the person who solves all five.

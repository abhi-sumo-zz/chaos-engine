# The Failure Library

Features this Library has:
1) 

## User Flow
1. User goes to a website, where he/she has the ability to select a scenario and a system to put under duress. The User can select from a set of systems to put under duress and a set of scenarios.

2. After selecting a scenario, the website starts running the scenario in a sandbox kubernetes cluster.

2a. Provisioning agent that starts up the cluster and the system along with the monitoring tools

2b. On user input, we start the failure scenario.

2c. Do we provide a kubeConfig or do we provide a cloud shell in the browser?

3. The user starts using the shell to debug the cluster. The timer and monitoring system continues until the SLA is repaired.

4. When the SLA is repaired, the user receives a scenario is over message, and is redirected to the webpage where they can see a replay of their debugging process, and a score of how well they did.


## Seeding the Library
1) All Kubernetes post-mortems can be converted to a scenario.
2) The Failure Stories blog posts can be conveted to scenarios.

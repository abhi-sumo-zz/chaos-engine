# Scenarios

A scenario is a failure situation. A scenario has the following properties:
1. The set of services and their configurations that need to be setup for the failure case.
1a. The set of services may contain custom images
1b. The set of services may contain standard off the shelf images.
1c. The set of services may contain bad actors (either via a mimic'd hack or a bad M&T actor - like a pod gone wild).

A scenario is not:
1. The tracking tool for how long it took to finish it.
2. The tool that sets up or initializes the scenario.
3. The tool that provides your grade / report.

The initial implementation of a Scenario can just be a helm chart that describes the services.
Pros of using a helm chart:
1. Standard Kubernetes install
2. Easy tear down, and setup.
3. Easy to maintain and read
4. An API most understand.

Cons of using a helm chart:
1. Custom images have to be accessible / managed somehow.
2. Still need an sdk for making bad actors in an easy manner.


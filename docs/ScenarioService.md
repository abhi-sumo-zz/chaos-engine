# Scenario Service
The Scenario Service handles the overall CRUD for scenarios.

It will allow you to:
1. Upload a HELM chart
2. Attach metadata to the helm chart such as: description, name, owner, public/private, expected time to complete.
3. Update helm charts once created.
4. See all your helm charts / scnearios.
5. Delete a scenario.
6. See the amount of times a scenario has been run.

Technology proposal:
1. Use S3 to store the Helm chart.
2. Use Postgres to store the metadata about the helm chart with the pointer to the s3.
3. Use a Kubernetes containerized typecript node server api-layer that accepts these CRUD calls. 

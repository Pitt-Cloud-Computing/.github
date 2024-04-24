# PCC - Medusa Commerce Server

## Deployment Diagram
<img width="981" alt="cs2060-final-project-diagram" src="https://github.com/Pitt-Cloud-Computing/.github/assets/57918989/45f9469e-5a8b-4c5e-b4ff-9c04e7f9c947">

## GCP Services
- Set Up A Google Organization + Google Workspace
  - Created “PCC - Medusa Commerce Project” and collaborated with multiple accounts.
- Used Identity and Access Management (IAM) And Workload Identity Pool
  - Delegated accesses to independent developers.
  - Created service accounts to use in the workload service pool with GitHub Actions.
- Stored Docker Images In Artifact Registry
  - Built and remotely stored Docker images using GitHub Actions.
  - Used the stored Docker images in GKE to spin up many containers.
- Hosted A Postgres Instance Using Cloud SQL
  - Connected the Postgres instance to the Medusa server.
- Hosted A Kubernetes Cluster Using GKE
  - Hosted many pods: Medusa server + admin, Medusa Next.js storefront template, Redis cache, load balancer, and persistent volumes.
  - Used Kubernetes keys in GKE for storing environment variables.
  - Used Storage Disks for creating the persistent volumes in GKE.
 
## Deployment Automation
- Used GitHub Actions Workflows
  - Set up a workflow to build and push the Docker image for Medusa Storefront 1 into Artifact Registry.
  - Set up a workflow to build and push the Docker image for Medusa Server into Artifact Registry.

## Video Presentation
- [Youtube Link](https://youtu.be/ptAaDbbii5E)

## References
- [Repo Link](https://github.com/Pitt-Cloud-Computing/pcc-docs)

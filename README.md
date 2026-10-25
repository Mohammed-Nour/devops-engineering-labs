# DevOps Engineering Labs

These are my DevOps labs from Innopolis University. I started with small web applications, then added Docker builds, CI pipelines, infrastructure configuration, and Kubernetes deployments.

The labs follow the [DevOps Core Course](https://github.com/inno-devops-labs/DevOps-Core-Course). I kept the original course introduction and grading rules in [COURSE.md](COURSE.md).

## Start here

| Topic | Files and walkthroughs |
|-------|------------------------|
| Applications and tests | [Python/Flask](app_python/README.md), [Go](app_go/README.md), and [React](app_react/README.md) |
| Containers | [Python Docker guide](app_python/DOCKER.md), [Go Docker guide](app_go/DOCKER.md), standard and distroless Dockerfiles |
| Continuous integration | [Python workflow](.github/workflows/python-app.yml) and [Go workflow](.github/workflows/go-app.yml) |
| Infrastructure as code | [Terraform configurations](terraform/) |
| Configuration management | [Ansible guide](ansible/ANSIBLE.md) and [roles](ansible/roles/) |
| Kubernetes and Helm | [Kubernetes guide](k8s/README.md), [Helm guide](k8s/helm/HELM.md), and [charts](k8s/helm/) |
| Secrets and configuration | [Vault and secrets exercise](k8s/11.md), [ConfigMaps exercise](k8s/12.md) |
| GitOps | [ArgoCD implementation walkthrough](k8s/13.md) and [application manifests](k8s/ArgoCD/) |
| Monitoring and logging | [Monitoring configuration](monitoring/) |
| Stateful workloads | [StatefulSet exercise](k8s/14.md) |

## What I worked on

- Built standard and distroless Docker images for the Python and Go applications.
- Added CI stages for security checks, linting, tests, and Docker image publishing.
- Used Ansible roles to install Docker and deploy the applications.
- Wrote Kubernetes manifests and Helm charts for configuration, secrets, and persistent workloads.
- Set up ArgoCD for dev and prod environments and tested how it handles configuration drift.

The guides include commands, screenshots, and output from the lab runs. Some workflows still reference lab branches, so check their configuration before reusing them.

## Explore the applications

Clone this repository:

```bash
git clone https://github.com/Mohammed-Nour/devops-engineering-labs.git
cd devops-engineering-labs
```

Choose an application and follow its setup guide:

- [Python application](app_python/README.md): installation, local execution, tests, and Docker.
- [Go application](app_go/README.md): local execution, tests, and container builds.
- [React application](app_react/README.md): frontend development and build instructions.

For the infrastructure labs, follow the relevant Ansible, Terraform, or Kubernetes guide with your own environment settings. Some older instructions use the repository name `S25-core-course-labs`; use the directory you cloned above instead.

## Related work

- [Wazuh incident-response research](https://github.com/Mohammed-Nour/mcp-server-wazuh/tree/main/research)
- [Vault with Kubernetes: four secret-management use cases](https://github.com/Mohammed-Nour/vault-secret-use-cases-project)
- [Portfolio](https://mohamadnourshahin.com/) · [LinkedIn](https://www.linkedin.com/in/mohamad-nour0/)

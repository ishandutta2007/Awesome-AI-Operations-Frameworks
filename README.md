# Awesome-AI-Operations-Frameworks

## Top AI Operations Frameworks Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Agent Harness Operations, Infrastructure Automation & Deployment Orchestration*  

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **AI Operations Frameworks**. These tools enable platform teams to run AI agent harnesses reliably—provisioning infrastructure, managing runtime state, orchestrating upgrades, and enforcing operational guardrails across development, staging, and production environments.



**Examples** include AWS Systems Manager, Azure Automation, Google Cloud Deployment Manager, Ansible Automation Platform, Puppet Enterprise, Chef Automate, SaltStack Enterprise, RunDeck, Terraform Cloud, and Spacelift (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, agent harness operations, and open infrastructure automation—ideal for platform engineers, SREs, and developers seeking transparent, vendor-independent AI operations.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[AWS Systems Manager](https://aws.amazon.com/systems-manager/)**  

  Unified operations hub for AWS and hybrid environments. Features **Patch Manager**, **Run Command**, **State Manager**, **Automation**, and **Session Manager**. **The most comprehensive managed operations platform** for AWS-native AI workloads.



- **[Azure Automation](https://azure.microsoft.com/en-us/products/automation/)**  

  Process automation with runbooks, configuration management, and update management. Integrates with Azure Monitor and Microsoft Defender.



- **[Google Cloud Deployment Manager](https://cloud.google.com/deployment-manager)**  

  Infrastructure deployment service for automating resource creation. Configuration files and templates define deployments across Compute Engine, Cloud Storage, and other services.



- **[Ansible Automation Platform (Red Hat)](https://www.redhat.com/en/technologies/management/ansible)**  

  Enterprise automation with **Ansible Automation Controller** (Tower), **Event-Driven Ansible**, and **Automation Hub**. **The most widely adopted agentless automation platform** for infrastructure and configuration.



- **[Puppet Enterprise](https://www.puppet.com/)**  

  Configuration management with desired-state enforcement, compliance scanning, and orchestration.



- **[Chef Automate](https://www.chef.io/)**  

  Infrastructure automation with compliance, application delivery, and visibility.



- **[SaltStack Enterprise (VMware)](https://www.vmware.com/products/application-platform.html)**  

  Event-driven infrastructure automation with remote execution and configuration management.



- **[RunDeck (PagerDuty)](https://www.rundeck.com/)**  

  Runbook automation with job scheduling, workflow orchestration, and access control. **The most focused runbook automation platform.**



- **[Terraform Cloud (HCP Terraform)](https://www.hashicorp.com/products/terraform)**  

  Managed IaC platform with workspaces, VCS integration, Sentinel/OPA policy as code, private module registry, and config-driven import. **Note**: resource-based pricing counts every resource in state—teams often find actual count is 3-4x assumed.



- **[Spacelift](https://spacelift.io/)**  

  Multi-IaC orchestration supporting Terraform, OpenTofu, Ansible, Kubernetes, Terragrunt, CloudFormation, and Pulumi. Features policy as code (OPA), stack dependencies, drift detection, and AI assistant with MCP server. Self-hosted option with multi-region DR.



## Open-Source GitHub Projects



- **[dsh-ops (T-Auto)](https://github.com/T-Auto/dsh-ops)**  

  **The operations framework explicitly designed for the DeepSeek Harness ecosystem** (open-source). **The reference implementation for agent harness operations.** Provides **deployment, runtime management, health monitoring, and upgrade orchestration** for DSH instances . **Opinionated defaults** for common operational patterns—service registration, log aggregation, graceful restart, and version pinning . **Extensible architecture** for custom operational workflows. **The emerging standard for AI harness operations.**



- **[Ansible](https://github.com/ansible/ansible)**  

  **The most widely adopted open-source configuration management and automation platform** (GPL-3.0). **63,000+ GitHub stars.** Agentless architecture via SSH. Supports cloud provisioning (AWS, Azure, GCP modules), configuration management, application deployment, and orchestration. **The foundation for AI operations automation** —manage GPU nodes, deploy model servers, and configure training clusters.



- **[Terraform](https://github.com/hashicorp/terraform)**  

  **Industry-standard IaC tool** (MPL-2.0) for provisioning cloud resources via HCL. **44,000+ GitHub stars.** Declarative configuration, plan/apply workflow, and extensive provider ecosystem covering AWS, Azure, GCP, and hundreds of services. **The foundation for AI infrastructure provisioning.**



- **[OpenTofu](https://github.com/opentofu/opentofu)**  

  **Open-source Terraform fork under Linux Foundation** (MPL-2.0). Created after HashiCorp's license change to BSL 1.1. Drop-in replacement with community governance. **25,000+ GitHub stars.** Features state encryption, early variable evaluation, and provider iteration.



- **[Kubernetes](https://github.com/kubernetes/kubernetes)**  

  **Container orchestration platform** (Apache-2.0) serving as cloud-native control plane. **113,000+ GitHub stars.** **The foundation for AI workload orchestration** —runs on-prem, in the cloud, in air-gapped environments, or in the field.



- **[Crossplane](https://github.com/crossplane/crossplane)**  

  **Open-source control plane turning Kubernetes into a universal cloud resource orchestrator** (Apache-2.0). **10,000+ GitHub stars.** Manages AWS, Azure, GCP, and on-prem resources as Kubernetes custom resources. **GitOps-driven infrastructure with continuous reconciliation and drift correction.**



- **[Pulumi](https://github.com/pulumi/pulumi)**  

  **Open-source IaC SDK using general-purpose programming languages** (Apache-2.0). **22,000+ GitHub stars.** Supports TypeScript, Python, Go, .NET, and Java. **100+ providers** including AWS, Azure, GCP, Kubernetes, and Cloudflare.



- **[Atlantis](https://github.com/runatlantis/atlantis)**  

  **Terraform pull request automation** (Apache-2.0) for GitOps workflows. **8,000+ GitHub stars.** Plan on PR, apply on merge.



- **[Cloud Custodian](https://github.com/cloud-custodian/cloud-custodian)**  

  **Multi-cloud governance rules engine** (Apache-2.0) for policy enforcement and cost optimization. **5,000+ GitHub stars.**



- **[KubeCost](https://github.com/kubecost/cost-analyzer)**  

  **Open-source Kubernetes cost monitoring** (Apache-2.0). **5,000+ GitHub stars.** Real-time cost visibility, allocation, and optimization for multi-cloud Kubernetes.



- **[Infracost](https://github.com/infracost/infracost)**  

  **Open-source cloud cost estimation for IaC** (Apache-2.0). **11,000+ GitHub stars.** Shows cost impact of Terraform changes in pull requests before apply.



- **[Argo CD](https://github.com/argoproj/argo-cd)**  

  **Declarative GitOps continuous delivery for Kubernetes** (Apache-2.0, CNCF Graduated). **18,000+ GitHub stars.** **The most widely adopted GitOps tool** for deploying AI workloads.



- **[Flux](https://github.com/fluxcd/flux2)**  

  **Open-source GitOps toolkit for Kubernetes** (Apache-2.0, CNCF Graduated). **6,000+ GitHub stars.** Alternative to Argo CD with tighter integration to GitOps Toolkit components.



- **[Argo Workflows](https://github.com/argoproj/argo-workflows)**  

  **Container-native workflow engine for Kubernetes** (Apache-2.0). **15,000+ GitHub stars.** DAG-based orchestration for ML training pipelines.



- **[Kubeflow](https://github.com/kubeflow/kubeflow)**  

  **ML toolkit for Kubernetes** (Apache-2.0) with training operator and pipeline orchestration.



- **[Volcano](https://github.com/volcano-sh/volcano)**  

  **Cloud-native batch scheduling system** (Apache-2.0) for high-performance workloads. CNCF Incubating project with gang scheduling and queue management.



### Additional Strong Open-Source Options



- **[Terragrunt](https://github.com/gruntwork-io/terragrunt)** — Thin Terraform wrapper (MIT) for DRY configurations and multi-environment orchestration.

- **[Puppet](https://github.com/puppetlabs/puppet)** — Open-source configuration management (Apache-2.0) with desired-state enforcement.

- **[Chef Infra](https://github.com/chef/chef)** — Open-source infrastructure automation (Apache-2.0).

- **[Salt](https://github.com/saltstack/salt)** — Open-source event-driven automation (Apache-2.0).

- **[Rundeck Community](https://github.com/rundeck/rundeck)** — Open-source runbook automation (Apache-2.0).

- **[Semaphore](https://github.com/semaphoreui/semaphore)** — Open-source Ansible/Terraform/Bash UI (MIT) for runbook orchestration.

- **[StackStorm](https://github.com/StackStorm/st2)** — Event-driven automation (Apache-2.0) for SOAR and ops workflows.

- **[N8n](https://github.com/n8n-io/n8n)** — Workflow automation (Sustainable Use License) with 400+ integrations.

- Community **n8n** workflows for AI operations alerting and deployment automation.



**Frameworks for building custom systems**: Combine **dsh-ops** for agent harness operations with **Ansible** for configuration management, **Terraform** or **OpenTofu** for infrastructure provisioning, **Kubernetes** with **Argo CD** for GitOps deployment, **Crossplane** for cloud resource orchestration, and **Infracost** for cost governance—creating a fully self-hosted, enterprise-grade AI operations platform.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- AI operations frameworks handling infrastructure and deployment credentials must follow security best practices (least privilege, short-lived credentials, audit logging) and comply with applicable regulations.

- **Open-source AI operations is mature and production-ready.** Ansible, Terraform, Kubernetes, and Argo CD are battle-tested at scale . **These are genuine alternatives to managed platforms.**

- **Agent harness operations is a new category.** dsh-ops exists because DSH instances require operational patterns—service registration, log aggregation, graceful restart, version pinning—that general-purpose tools do not handle out of the box . **The operations framework is the missing layer between the harness and the infrastructure.**

- **IaC licensing matters.** Terraform moved to BSL 1.1 in 2023, prompting the OpenTofu fork under Linux Foundation. **OpenTofu is MPL-2.0 and community-governed** —choose based on your licensing requirements .

- **Resource-based pricing can surprise you.** HCP Terraform's resource-based pricing counts every resource in state—teams often find their actual count is 3-4x assumed . **Measure before committing to tiers.**

- Self-hosted open-source solutions require proper security hardening, state file protection, and ongoing maintenance. **Infrastructure automation is security-critical**—state files contain secrets and must be encrypted and access-controlled.



---



**Made for platform engineers, SREs, and developers building transparent AI operations solutions.**  

Let's make AI Operations Frameworks more open, data-driven, and agent-aware.

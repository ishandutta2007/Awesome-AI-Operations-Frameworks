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

| Platform | Company Scale (Valuation / Revenue) | Description | Pricing | Free Tier Limits |
| :--- | :--- | :--- | :--- | :--- |
| **[Azure Automation](https://azure.microsoft.com/en-us/products/automation/)** | **~$3.1T** Market Cap (Microsoft) / **$245B+** Revenue | Cloud-based process automation, runbooks, configuration management, and update orchestration across hybrid setups. | Process automation overage starts at **$0.002 per job run minute**; watcher overage at **$0.002 per hour**. | **Free forever**: **500 job run minutes** per subscription per month and **744 watcher hours** per month (capped at 50 concurrent jobs). |
| **[AWS Systems Manager](https://aws.amazon.com/systems-manager/)** | **~$2.0T** Market Cap (Amazon) / **$107B+** AWS Revenue | Unified operations hub for AWS and hybrid environments with Patch Manager, Run Command, State Manager, and Session Manager. | Core management is free; Advanced Parameter Store starts at **$0.05 per parameter/month** + $0.05/10k interactions; On-prem/hybrid instances managed at no additional SSM license fee. | **Free forever**: Core management features on EC2 & hybrid nodes are 100% free; up to **10,000 standard parameters** per region (up to 4 KB each) and standard throughput API calls. |
| **[Google Cloud Deployment Manager](https://cloud.google.com/deployment-manager)** | **~$2.0T** Market Cap (Alphabet) / **$40B+** GCP Revenue | Declarative infrastructure deployment service for defining and provisioning Google Cloud resources via YAML templates. | **$0.00** service charge (100% free tool; users only pay for the underlying Google Cloud compute, disk, and network resources provisioned). | **Free forever**: Tool usage is completely free up to **1,000 active deployments** per project, **1,000 write API requests/day**, and 20 requests/sec. |
| **[SaltStack Enterprise (VMware / Tanzu)](https://www.vmware.com/products/application-platform.html)** | **~$800B** Market Cap (Broadcom) / **$51B+** Revenue | Event-driven infrastructure orchestration, compliance management, and remote execution across multi-cloud environments. | Packaged within VMware Cloud Foundation (VCF) / Tanzu Automation starting at **~$450 to $650 per core/year** (subject to 16 cores/CPU & 72 cores order minimums); standalone node packages via custom enterprise quote. | **No standard self-service free tier**; available via **sales-assisted 30-day proof-of-concept (PoC) / guided sandbox trial**. Free alternative: Salt Open (Apache 2.0, unlimited nodes, CLI only). |
| **[Ansible Automation Platform (Red Hat)](https://www.redhat.com/en/technologies/management/ansible)** | **~$200B** Market Cap (IBM) / Red Hat acquired for **$34B** | Enterprise automation suite featuring Automation Controller (Tower), Event-Driven Ansible, private automation hub, and analytics. | Standard Tier starts at **~$13,000 to $17,000 per year** per 100 managed nodes (pack); Premium 24x7 Tier starts at **~$17,500 to $19,250 per year** per 100 managed nodes. | **60-day free trial** with access to Automation Controller and Hub, limited to **up to 100 managed nodes** (self-supported). Free alternative: open-source Ansible Core (CLI, unlimited). |
| **[Terraform Cloud (HCP Terraform)](https://www.hashicorp.com/products/terraform)** | **$6.4B** Acquisition Valuation (IBM / HashiCorp) | Managed infrastructure-as-code platform with remote state management, VCS-driven runs, private registry, and Sentinel/OPA policies. | Essentials starts at **$0.10 per managed resource/month**; Standard plan starts at **$0.47 per managed resource/month**; Premium starts at **$0.99 per managed resource/month**. | **Free forever**: Up to **500 managed resources under management (RUM)**, unlimited users, and 1 concurrent run. |
| **[Puppet Enterprise](https://www.puppet.com/)** | **~$3.0B+** Valuation (Perforce Software backed by Clearlake & Francisco Partners) | Configuration management platform providing desired-state enforcement, automated compliance auditing, and continuous orchestration. | Standard Support plans start at **~$112 to $166 per node/year**; Premium plans start at **~$199 to $250 per node/year** (annual subscription, multi-node discounts available). | **Free forever**: Fully functional on **up to 10 nodes** with no expiration date or license key required. |
| **[Chef Automate](https://www.chef.io/)** | **~$1.8B** Market Cap (Progress Software, NASDAQ: PRGS) | Infrastructure automation, compliance visibility, and full-stack DevOps workflow management dashboard. | Business Tier starts at **$59 per node/year**; Enterprise Automate / Enterprise Plus tiers start at **$189 per node/year** (annual contract). | **60-day free trial** with full access to Chef Automate, compliance auditing, and configuration workflows (features shut down upon trial expiration). |
| **[RunDeck (PagerDuty)](https://www.rundeck.com/)** | **~$1.3B** Market Cap (PagerDuty, NYSE: PD) / **$493M** FY26 Revenue | Runbook automation platform for self-service operational workflows, automated incident remediation, and access control. | PagerDuty Runbook Automation (SaaS) starts at **$125 per user/month + platform fee**; Self-Hosted Enterprise starts at custom annual contracts (~$50,000+/year). | **14-day free trial** of PagerDuty Operations Cloud / Runbook Automation. Free alternative: Rundeck Community Edition (Apache 2.0, unlimited self-hosted nodes/jobs, unmanaged). |
| **[Spacelift](https://spacelift.io/)** | **~$204M** Valuation ($87M+ funding raised) | Specialized multi-IaC orchestration platform supporting OpenTofu, Terraform, Ansible, Pulumi, Kubernetes, and CloudFormation with OPA governance. | Starter+ plan starts at **$20,000 per year** (includes 1 private worker and unlimited users); Business and Enterprise tiers are custom quote-based. | **Free forever**: Up to **2 users**, 1 concurrent run, unlimited public/private stacks, and standard VCS integrations. Paid features available on a **14-day free trial**. |



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

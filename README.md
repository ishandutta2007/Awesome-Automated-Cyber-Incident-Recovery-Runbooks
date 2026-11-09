# Awesome-Automated-Cyber-Incident-Recovery-Runbooks

# Awesome-Automated-Cyber-Incident-Recovery-Runbooks

## Top Automated Cyber Incident Recovery Runbooks Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Cyber Recovery Automation, Isolated Recovery Environments & Ransomware-Resilient Orchestration*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Automated Cyber Incident Recovery Runbooks**. These tools orchestrate recovery from cyberattacks—especially ransomware—by automating clean-room validation, boot-order sequencing, threat scanning, and post-recovery scripts, while ensuring recovery points predate compromise.

**Examples** include Druva Cyber Recovery Runbooks, Zerto Cyber Recovery Plans, Veeam Disaster Recovery Orchestrator, Rubrik Cyber Recovery, Cohesity SiteContinuity, Commvault Cleanroom Recovery, CloudEndure Disaster Recovery, AWS Elastic Disaster Recovery, Azure Site Recovery, and IBM Cyber Resiliency (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosted recovery orchestration, infrastructure-as-code disaster recovery, ransomware decryption tooling, and CI-native recovery validation—ideal for platform teams, SREs, security engineers, and developers building transparent, vendor-neutral cyber resilience workflows.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS/Hosted Platforms](#saashosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## Sector Overview & Market Dynamics

The global Cyber Recovery and Disaster Recovery as a Service (DRaaS) market is valued at approximately **$13 billion to $17 billion** and is projected to expand at an annual growth rate (CAGR) of **16% to 23%** into the next decade. The sector exhibits a bifurcated market structure: it is **highly concentrated** at the underlying infrastructure layer dominated by hyperscalers (Microsoft, AWS, and Google), yet **moderately fragmented** at the cyber-recovery orchestration, cleanroom validation, and specialized software layer where independent vendors, enterprise backup leaders, and agile security platforms compete actively.

## SaaS/Hosted Platforms

| Company / Product | Company Size (Valuation / Revenue) | Starting Price (Specific Tier) | Free Tier Limits / Free Trial Policy | Key Cyber Recovery Capabilities |
| :--- | :--- | :--- | :--- | :--- |
| **[Azure Site Recovery](https://azure.microsoft.com/en-us/products/site-recovery)** | **$3.1T+ Market Cap** / $245B+ Annual Revenue (Microsoft) | **$25.00/instance/month** (replicated to Azure) or **$16.00/instance/month** (replicated to customer-owned sites) | **31-Day Free Trial per instance** (first 31 days free for every protected instance; compute/storage consumed during failovers billed separately) | Ordered VM groups, native Azure Automation runbook orchestration, scripted post-failover validation for multi-tier apps [citation:9][citation:18]. |
| **[AWS Elastic Disaster Recovery](https://aws.amazon.com/disaster-recovery/)** | **$2.1T+ Market Cap** / $600B+ Annual Revenue (Amazon / AWS) | **$0.028/server/hour** (~$20.44/server/month base software license) | **No permanent free tier**; introductory AWS free trial promotions provide up to 90 days per server for eligible new accounts (EBS/EC2 drill infrastructure billed separately) | Continuous block-level replication, sub-second RPO point-in-time recovery, automated non-disruptive recovery drills, cross-Region failover [citation:8]. |
| **[CloudEndure Disaster Recovery (AWS)](https://docs.cloudendure.com/)** | **$2.1T+ Market Cap** / $600B+ Annual Revenue (Amazon / AWS) | **$0.028/server/hour** (~$20.44/server/month base software license) | **No permanent free tier**; trial evaluation accessible via AWS account setup (replicated staging compute/EBS storage billed separately) | Continuous block-level replication and automated recovery orchestration for physical, virtual, and cloud workloads [citation:7]. |
| **[IBM Cyber Resiliency (Safeguarded Copy)](https://www.ibm.com/)** | **$210B+ Market Cap** / $62B+ Annual Revenue (IBM) | **Included with IBM Storage Virtualize base license**; advanced IBM Storage Defender software suite starts at ~$65.00/TB/year | **No permanent free tier**; offers structured **14-day on-premises proof-of-concept (PoC) / test-drive** program and free cyber resilience assessment | Immutable Safeguarded Copy snapshots, air-gapped copies, cryptographic verification, and surgical isolated recovery for z/OS and distributed storage [citation:10]. |
| **[HPE Zerto Cyber Recovery Plans](https://www.zerto.com/)** | **$25B+ Market Cap** / $29B+ Annual Revenue (Hewlett Packard Enterprise) | **$33.00/VM/month** (cloud migration tier) to **$83.33/VM/month** ($1,000/VM/year enterprise baseline) | **30-Day Free Trial** up to 10 VMs via Zerto In-Cloud (or 14-day trial for up to 15 VMs on enterprise packages) | Platform-native cyber recovery plans, ordered multi-VPG orchestration, journaling to recover to clean points pre-dating compromise [citation:2]. |
| **[Veeam Disaster Recovery Orchestrator](https://www.veeam.com/)** | **$15B Valuation** / $1.7B+ ARR (Veeam Software) | **$12.92/workload/month** ($155/workload/year under Veeam Universal License packs) | **Free forever plan: Community Edition up to 10 workloads**; full enterprise orchestration trial available for **30 days** | Automated recovery plan orchestration, isolated test labs (DataLabs), compliance-ready dynamic DR documentation, malware scanning [citation:3][citation:15]. |
| **[Rubrik Cyber Recovery](https://www.rubrik.com/)** | **$13.9B Market Cap** / $1.09B Subscription ARR (Rubrik, Inc.) | **$130.00/TB/month** (Backup Enterprise Terabyte list baseline; multi-year enterprise contracts start at ~$50,000/year) | **No permanent free tier**; structured **30-day Proof-of-Concept (PoC) / trial** available through enterprise sales team | Cleanroom Live Mount threat hunting, anomaly-filtered snapshot selection, boot-order sequencing, automated quarantine [citation:4]. |
| **[Cohesity SiteContinuity](https://www.cohesity.com/)** | **$7B–$8B Valuation** / $1.7B+ Combined Revenue (Cohesity) | **$83.33/TB/month** ($1,000/TB/year baseline enterprise commitment; AWS Marketplace starts at $2,425/month for 10 BETB) | **30-Day Free Trial** for Cohesity DataProtect / BaaS cloud orchestration (underlying cloud infrastructure costs apply) | Unified backup and automated DR, policy-driven failover/failback orchestration, isolated recovery testing across hybrid clouds [citation:5]. |
| **[Commvault Cleanroom Recovery](https://documentation.commvault.com/)** | **$5.5B–$6.6B Market Cap** / $996M Annual Revenue (Commvault) | **$8.17/VM/month** ($98/VM/year hybrid VM pack) or **$58.50/TB/month** for SaaS cloud storage; Cleanroom capacity starts in 10 TB recovery blocks | **30-Day Free Trial** (no credit card required) for Commvault Cloud SaaS and Cleanroom Recovery testing | AWS cleanroom automated provisioning, integrated Microsoft Defender scanning, custom validation scripts, prioritized VM boot sequencing [citation:6]. |
| **[Druva Cyber Recovery Runbooks](https://www.druva.com/)** | **$2B Peak Valuation** / $200M+ SaaS ARR (Druva) | **$8.00/user/month** (SaaS/endpoint tier) or **$200.00/credit/month** (1 credit = 1 TB deduplicated storage/month) | **30-Day Free Trial** (extendable up to 60 days via tenant admin) with full access to SaaS resiliency workflows | Automated Scheduled Cyber Recovery Testing, Live Incident Recovery orchestration, Isolated Recovery Environment (IRE) and IOC scanning [citation:1][citation:13]. |

## Open-Source GitHub Projects

- **[Relax-and-Recover (ReaR)](https://github.com/rear/rear)**  
  Leading open-source disaster recovery and system migration framework for Linux, producing bootable rescue images with support for Bacula, Borg, Duplicity, rsync, and many enterprise backup backends [citation:16].

- **[0xelitesystem/incident-response-runbooks](https://github.com/0xelitesystem/incident-response-runbooks)**  
  Ten incident response runbooks (ransomware, leaked keys, data exfiltration, supply-chain compromise) following a consistent skeleton: trigger, containment, eradication, recovery, post-incident [citation:11].

- **[Stronghold](https://github.com/mehdi-arfaoui/Stronghold)**  
  DRP-as-Code platform that discovers infrastructure, builds dependency graphs, detects single points of failure, generates recovery plans, and validates through micro-tests [citation:12].

- **[cloud-dr-orchestrator](https://github.com/Kobeep/cloud-dr-orchestrator)**  
  Multi-cloud disaster recovery orchestrator with automated backup scheduling, encrypted uploads, and restore workflows targeting Oracle Cloud Free Tier [citation:17].

- **[multicloud-disaster-recovery](https://github.com/bukx/multicloud-disaster-recovery)**  
  Reference architecture for cross-cloud failover across AWS, Azure, and GCP using Terraform, Pulumi, Ansible, Route 53, and Datadog for centralized visibility [citation:27].

- **[lockbit-rescue](https://github.com/Saddytech/lockbit-rescue)**  
  Toolkit for recovering LockBit 3.0 encrypted files without paying ransom, exploiting Salsa20 keystream reuse across file batches [citation:19].

- **[c3rb3r-rescue](https://github.com/soimy/c3rb3r-rescue)**  
  Evidence-preserving recovery for C3RB3R/.L0CK3D ransomware on Synology DSM, including RAM key extraction, process freezing, and Btrfs copy-on-write recovery routes .

- **[c3rb3r-btrfs-recovery](https://github.com/crt106/c3rb3r-btrfs-recovery)**  
  Keyless recovery of C3RB3R-encrypted Synology/Btrfs files by mapping rewritten bytes back to surviving copy-on-write extents via the extent tree [citation:29].

- **[DaliBackup-OSS](https://github.com/daliranas/DaliBackup-OSS)**  
  Lightweight sovereign backup and DR orchestration for Hyper-V, Proxmox VE, and IMAP mailboxes with embedded SQLite and AES-256-GCM encryption [citation:21].

- **[Azure Automation Runbooks (Site Recovery Integration)](https://github.com/MicrosoftDocs/azure-docs/blob/main/articles/site-recovery/site-recovery-runbook-automation.md)**  
  Reference implementation and context schema for invoking Azure Automation runbooks within Site Recovery recovery plans for post-failover configuration [citation:28].

### Additional Strong Open-Source Options

- **[Bacula](https://github.com/bacula-web/bacula-web)** and **[Bareos](https://github.com/bareos/bareos)** for open-source enterprise backup with recovery orchestration hooks.
- **[BorgBackup](https://github.com/borgbackup/borg)** and **[Duplicity](https://github.com/duplicity/duplicity)** for deduplicated, encrypted backups usable in custom recovery pipelines.
- **[Velero](https://github.com/vmware-tanzu/velero)** for Kubernetes cluster backup and restore orchestration.
- **[LitmusChaos](https://github.com/litmuschaos/litmus)** and **[Chaos Mesh](https://github.com/chaos-mesh/chaos-mesh)** for recovery drill automation and failure injection.
- Many community **DRP-as-Code** templates and **Terraform/Pulumi recovery modules** for cloud-native failover.

**Frameworks for building custom systems**: Combine **ReaR**, **Stronghold**, **Velero**, and **GitHub Actions** with **Allure** or **Prometheus** for end-to-end cyber recovery validation pipelines.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Cyber recovery tooling must be validated against your organization's RTO/RPO requirements and regulatory obligations.
- Self-hosted open-source solutions require proper isolation, access control, and regular recovery testing.

---

**Made for SREs, security engineers, platform teams, and cyber resilience architects.**  
Let's make cyber incident recovery more open, automated, and provable.

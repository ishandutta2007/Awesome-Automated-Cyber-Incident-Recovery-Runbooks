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
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Druva Cyber Recovery Runbooks](https://www.druva.com/)**  
  Automated threat-aware recovery with Scheduled Cyber Recovery Testing and Live Incident Recovery, using Isolated Recovery Environment (IRE) and IOC scanning before production restore [citation:1][citation:13].

- **[HPE Zerto Cyber Recovery Plans](https://www.zerto.com/)**  
  Platform-native recovery plans for cyber scenarios, guiding teams to clean recovery points that predate corruption, with ordered multi-VPG orchestration [citation:2].

- **[Veeam Disaster Recovery Orchestrator](https://www.veeam.com/)**  
  One-click orchestration plans with automated testing, isolated test labs, and compliance-ready documentation for VMware and Azure recovery [citation:3][citation:15].

- **[Rubrik Cyber Recovery](https://www.rubrik.com/)**  
  Recovery plans for Hyper-V and Azure Local with boot-order sequencing, clean-room Live Mount investigation, and anomaly-filtered snapshot selection [citation:4].

- **[Cohesity SiteContinuity](https://www.cohesity.com/)**  
  Integrated backup and automated disaster recovery with policy-driven failover and failback orchestration across on-premises and cloud [citation:5].

- **[Commvault Cleanroom Recovery](https://documentation.commvault.com/)**  
  Runbooks for AWS cleanroom sites with threat scanning, Windows Defender integration, custom validation scripts, and priority-based VM boot sequencing [citation:6].

- **[CloudEndure Disaster Recovery (AWS)](https://docs.cloudendure.com/)**  
  Continuous replication and automated recovery orchestration for physical, virtual, and cloud servers (now part of AWS Elastic Disaster Recovery) [citation:7].

- **[AWS Elastic Disaster Recovery](https://aws.amazon.com/disaster-recovery/)**  
  Continuous replication with point-in-time recovery, cross-Region failover, and automated drill execution for EC2 and on-premises workloads [citation:8].

- **[Azure Site Recovery](https://azure.microsoft.com/en-us/products/site-recovery)**  
  Recovery plans with ordered VM groups, Azure Automation runbook integration, and scripted post-failover actions for multi-tier applications [citation:9][citation:18].

- **[IBM Cyber Resiliency (Safeguarded Copy)](https://www.ibm.com/)**  
  Immutable Safeguarded Copy snapshots with enterprise-level recovery guarantees, air-gapped copies, and surgical recovery for z/OS and distributed environments [citation:10].

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

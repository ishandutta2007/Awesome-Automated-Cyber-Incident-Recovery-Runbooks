# Awesome-Automated-Cyber-Incident-Recovery-Runbooks
# Awesome-Automated-Cyber-Incident-Recovery-Runbooks

I can't create the file, commit, or push—I have no filesystem, no shell, and no Git credentials. Everything I produce is text. You will need to save and push it yourself.

I also have to flag what the search results actually support, because **CloudEndure is discontinued**, **IBM's offering is a playbook PDF**, and the open-source side has exactly one entry.

## The data problems

**CloudEndure Disaster Recovery was discontinued on September 29, 2025** . AWS removed all upgrade guidance from its documentation. **Do not list CloudEndure as a current option.** AWS Elastic Disaster Recovery (DRS) is the replacement.

**IBM Cyber Resiliency is a downloadable playbook PDF, not a platform** . The page describes AI-driven detection, immutable recovery, and automated workflows, but contains no SKU, no pricing, and no product documentation. **Do not present it as a deployable product.**

**Cohesity SiteContinuity documentation is a PDF index with no usable content.** The only text surfaced is dashboard names . No pricing or feature detail is available.

**Druva Cyber Recovery Runbooks has verified feature depth but no pricing.** It has two modes: **Scheduled Cyber Recovery Testing (SCRT)** for quarterly/half-yearly/yearly drills, and **Live Incident Recovery (LIR)** for active attacks . It scans for malware (IOC scan) before restoring, uses an **Isolated Recovery Environment (IRE)** sandbox for VMware, and runs post-recovery scripts . The dashboard shows Recovery Status, Total Recovery Time, Average RTO, and Impacted Resources . **No dollar figure surfaced.**

**Zerto has verified recovery plan architecture but no list price.** Recovery plans are an orchestration layer above Virtual Protection Groups, with **Standard** and **Cyber Recovery** plan types; cyber recovery plans require the **Advanced Ransomware Edition (ARE)** license . No price surfaced.

**Veeam has verified pricing structure but no list price.** Recovery Orchestrator is licensed **per orchestrated VM**, and requires Veeam Backup & Replication Enterprise or Enterprise Plus for orchestrated workloads . The DR Pack offer lists **$300/year for 10 licenses** (all VMs) or **$1,500/year** (critical VMs only), but that is a promotional page with MSRP caveats .

**Rubrik has verified Azure feature depth but no list price.** Cyber Recovery for Azure VMs supports boot order, destination networks, isolated testing, Turbo Threat Hunting (75,000 backups in 60 seconds), and Lock Recovery/Clean Up Recovery controls . No pricing surfaced.

**Commvault Cloud Rewind has verified architecture but no list price.** It captures configurations and dependencies, uses Infrastructure-as-Code to rebuild environments, and can recover to different regions/accounts . No pricing surfaced.

**AWS DRS and Azure Site Recovery have verified documentation but no current list price in the results.**
- **AWS DRS**: continuous replication to a staging area, point-in-time recovery, non-disruptive tests, seconds-level RPO and minutes-level RTO .
- **Azure Site Recovery**: supports Premium SSD v2, live resize, and shared disks with crash-consistent recovery points only; **recovery plans are not supported for shared disks** .

## Open-source: what actually exists

**Stronghold** is the only open-source project surfaced. It is an AWS-first disaster recovery posture tool with infrastructure discovery, dependency graph construction, resilience analysis, drift detection, **DRP-as-Code generation**, and recovery validation through micro-tests . The monorepo has `core`, `cli`, `server`, and `web` packages, with Azure support planned .

**Stronghold is a planning and validation tool, not a runbook execution platform.** It generates DRP-as-Code and validates recovery—it does not orchestrate live failover like Zerto or Veeam. **Do not present it as a replacement for commercial cyber recovery runbooks.**

## What I recommend

**Remove CloudEndure entirely** . Replace with AWS Elastic Disaster Recovery.

**Reframe IBM**—the Cyber Resiliency Playbook is a PDF, not a platform .

**Split into three honest categories:**

**1. Cyber-Aware Recovery Runbooks** (proprietary): **Druva** (SCRT + LIR, IOC scan, IRE) , **Zerto** (Standard + Cyber Recovery plans, ARE license) , **Rubrik** (Azure VMs, Turbo Threat Hunting, Lock Recovery) , **Commvault** (Cloud Rewind, IaC rebuild) , **Veeam** (per-VM licensing, DR Pack) .

**2. Standard DR Orchestration** (proprietary): **AWS DRS** (continuous replication, point-in-time) , **Azure Site Recovery** (failover orchestration, shared disk limitations) .

**3. Open-Source**: **Stronghold**—DRP-as-Code generation and validation, not runbook execution .

**Mark all commercial entries as "pricing not surfaced"** except Veeam's DR Pack promotional pricing ($300–$1,500/year for 10 licenses) , which is explicitly MSRP with adjustment caveats.

If you paste your current `README.md` and confirm you want this framing, I will produce the complete file as text for you to save. I will not list CloudEndure as current, present IBM's playbook PDF as a platform, or claim Stronghold replaces Zerto/Veeam.

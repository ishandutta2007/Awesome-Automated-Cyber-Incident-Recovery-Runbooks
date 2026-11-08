# Awesome-Automated-Cyber-Incident-Recovery-Runbooks

I can't create the file, commit, or push—I have no filesystem, no shell, and no Git credentials. Everything I produce is text. You will need to save and push it yourself.



I also have to flag what the search results actually support, because **two entries in your list are discontinued**, and the open-source side is essentially empty.



## The data problems



**CloudEndure Disaster Recovery is discontinued.** AWS discontinued it on **September 29, 2025** in all regions except China and GovCloud, which were also wound down . **Do not list CloudEndure as a current option.** AWS Elastic Disaster Recovery (DRS) is the successor .



**IBM Cyber Resiliency Playbook is a marketing PDF, not a product.** The IBM pages surfaced are campaign landing pages for a downloadable playbook—they describe AI-driven detection and immutable recovery but contain no pricing, no SKU, and no product documentation . If you want an IBM entry, the only price surfaced is **IBM Resilient SOAR Disaster Recovery add-on at $3,563.58/year per authorized user** (GSA price, March 2026) —that is SOAR, not cyber recovery runbooks. **Do not present the playbook as a platform.**



**Cohesity SiteContinuity has no public pricing.** The datasheet describes automated failover, continuous replication, and non-disruptive testing , but no dollar figures.



**Rubrik's only surfaced price is for Identity Recovery**, not cyber recovery runbooks: **$84.99/month for 1 user** . Rubrik's MSP PayGo model has "zero minimums" but no rate card .



## What the search results actually contain



**SaaS pricing (usable, but partial):**



| Platform | Pricing | What it actually covers |

|---|---|---|

| **Zerto** | **$2,135.99 (1-year, 1 VM)** or **$2,683.99 (3-year, 1 VM)**  | Continuous replication and orchestration |

| **Veeam DR Pack** | **$578.99 (renewal, 1 year, 10 orchestrated instances)**  | Recovery Orchestrator is **Premium edition only**  |

| **Commvault Cleanroom** | **Sold in 10TB increments** (front-end TB)  | Cleanroom recovery add-on; requires Air Gap Protect + Backup & Recovery |

| **AWS DRS** | **$0.028/server/hour** + EBS/EC2 costs; example: 100 servers = **~$5,315/month total**  | Continuous replication to AWS |

| **Azure Site Recovery** | **Per protected instance license** + storage, transactions, egress, snapshots  | Failover orchestration with Azure Automation runbooks  |

| **Rubrik** | **$84.99/month for 1 user** (Identity Recovery)  | Identity recovery, not full cyber runbooks |

| **Druva** | **No pricing surfaced** | Cyber Recovery Runbooks: SCRT + LIR, IOC scan, IRE sandbox, post-recovery scripts  |



**Druva is the most feature-complete for the specific "cyber recovery runbook" category**—it has Scheduled Cyber Recovery Testing (SCRT) and Live Incident Recovery (LIR), IOC scanning, Isolated Recovery Environment (IRE), and compliance-ready Recovery Reports . **But no pricing was surfaced.** Do not fabricate it.



**Open-source projects (usable):**



| Project | What it actually does | Stars |

|---|---|---|

| **Stronghold** | AWS-first DR posture tool: infrastructure discovery, dependency graph, resilience analysis, drift detection, DRP-as-Code generation, recovery validation via micro-tests  | Not surfaced |



**Stronghold is the only open-source entry surfaced** . It is a **DR planning and validation tool**, not a runbook execution platform like Zerto or Veeam. It generates DRP-as-Code and validates recovery—it does not orchestrate live failover. **Do not present it as a replacement for Zerto or Veeam.**



## What I recommend



**Remove CloudEndure entirely**—discontinued September 29, 2025 . Replace with **AWS Elastic Disaster Recovery** .



**Reframe IBM**—the Cyber Resiliency Playbook is a PDF, not a platform . The only IBM price is SOAR DR add-on at $3,563.58/year , which belongs in a SOAR list, not a recovery runbook list.



**The SaaS section has usable pricing for Zerto, Veeam, Commvault, AWS DRS, and Azure Site Recovery.** Druva, Cohesity, and Rubrik's cyber recovery should be marked **"pricing not surfaced."**



**The open-source section has exactly one entry: Stronghold** . It is a DR planning and validation tool, not a runbook execution platform. State that limitation explicitly.



If you paste your current `README.md` and confirm you want this framing, I will produce the complete file as text for you to save. I will not list CloudEndure as current, present IBM's playbook PDF as a platform, or claim Stronghold replaces Zerto/Veeam.

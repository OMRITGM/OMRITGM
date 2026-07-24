<h1 align="center">Omri Elcharizi</h1>

<p align="center">
  <a href="https://omrielcharizi.com"><img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=18&pause=1000&color=3A9BC7&center=true&vCenter=true&width=560&lines=System+Administrator+building+the+bridge+to+DevOps;Proxmox+%2B+Terraform+%2B+Ansible%2C+run+like+production;I+maintain+the+server+and+write+the+UI+that+talks+to+it" alt="typing tagline"></a>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/omri-elcharizi-788a931a9"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:omri7779@gmail.com"><img src="https://img.shields.io/badge/Email-omri7779%40gmail.com-D14836?style=flat&logo=gmail&logoColor=white" alt="Email"></a>
  <a href="https://omrielcharizi.com"><img src="https://img.shields.io/badge/Portfolio-omrielcharizi.com-3a9bc7?style=flat&logo=googlechrome&logoColor=white" alt="Portfolio"></a>
  <a href="https://omrielcharizi.com"><img src="https://img.shields.io/badge/CV-Download-1a7f37?style=flat&logo=googledocs&logoColor=white" alt="Download CV"></a>
</p>

---

Three years as a systems technician and team lead in an operational Air Force environment: Windows Server, Active Directory, VMware vSphere, and endpoint security for hundreds of users under SLA, where a mistake reaches real people fast. I'm moving that discipline into DevOps: a Proxmox homelab run the same way production should be, Infrastructure-as-Code, and an AWS Solutions Architect certification in progress.

I maintain the servers and I write the interfaces that talk to them, so I debug the whole stack, not just my half of it.

## Experience

**Frontend & Infrastructure &#183; Reserves**, Maintenance Squadron, Israeli Air Force &#183; Today to Apr 2026
Client-side development alongside the technical role: rebuilding screens for a daily-use system, adding validation scripts, turning end-user feedback into interface changes.

**Systems Technician &#183; Team Lead**, Maintenance Squadron, Israeli Air Force &#183; Aug 2023 to Apr 2026
Led a team of technicians in a multi-site operational environment. Active Directory account and permission management, Windows Server 2012/2016 and Linux maintenance over SSH, VMware vSphere and IBM enterprise storage support, endpoint security with McAfee ePO (Trellix), support for hundreds of users under SLA.

## Certifications & education

- AWS Certified Solutions Architect, Associate: in progress
- DevOps Digital, Ecomschool: in progress (final certificate pending two exams)
- Diploma, Electronics & Computer Engineering, HaMechina HaTechnologit Mekif Alef, Ashdod (2023)

## Stack

**Systems & networking**
<p>
  <img src="https://img.shields.io/badge/Windows_Server-0078D6?style=flat&logo=windows&logoColor=white" alt="Windows Server">
  <img src="https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black" alt="Linux">
  <img src="https://img.shields.io/badge/Active_Directory-0078D4?style=flat&logo=microsoftazure&logoColor=white" alt="Active Directory">
  <img src="https://img.shields.io/badge/VMware_vSphere-607078?style=flat&logo=vmware&logoColor=white" alt="VMware">
</p>

**Infrastructure as code**
<p>
  <img src="https://img.shields.io/badge/Proxmox_VE-E57000?style=flat&logo=proxmox&logoColor=white" alt="Proxmox">
  <img src="https://img.shields.io/badge/Terraform-844FBA?style=flat&logo=terraform&logoColor=white" alt="Terraform">
  <img src="https://img.shields.io/badge/Ansible-EE0000?style=flat&logo=ansible&logoColor=white" alt="Ansible">
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white" alt="Docker">
  <img src="https://img.shields.io/badge/AWS-232F3E?style=flat&logo=amazonaws&logoColor=white" alt="AWS">
</p>

**Automation & observability**
<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/n8n-EA4B71?style=flat&logo=n8n&logoColor=white" alt="n8n">
  <img src="https://img.shields.io/badge/Prometheus-E6522C?style=flat&logo=prometheus&logoColor=white" alt="Prometheus">
  <img src="https://img.shields.io/badge/Grafana-F46800?style=flat&logo=grafana&logoColor=white" alt="Grafana">
</p>

## Projects

**[homelab-as-code](https://github.com/OmriTGM/homelab-as-code)** &#183; [![CI](https://github.com/OmriTGM/homelab-as-code/actions/workflows/ci.yml/badge.svg)](https://github.com/OmriTGM/homelab-as-code/actions/workflows/ci.yml)
Terraform provisions 15 LXC containers from one data map, Ansible configures them, and an exporter I wrote publishes state to Prometheus. The `containers` map that creates a container is the same one that labels its metrics, so the lab and its monitoring can't drift apart. 23 tests, five documented ADRs, gitleaks in CI, and a known-limitations section that says what's actually still rough.

**[mail-classifier](https://github.com/OmriTGM/mail-classifier)**
n8n polls Gmail every 15 minutes, sends each new email to a local LLM (qwen3:14b) on an RTX 3060, and applies a matching label. The classify request retries twice with a 5-second gap and continues on failure, so one bad response doesn't stall the queue. Zero API cost since the model runs at home.

## Home lab

<p align="center">
  <img src="assets/homelab-architecture.svg" alt="Proxmox homelab architecture: host with RTX 3060 passthrough, 15 LXC containers grouped into AI/automation, media stack, infra/platform, and home">
</p>

Single node, 15 isolated LXC containers, one RTX 3060 passed through for local inference. Scheduled backups, SMART monitoring, a reverse proxy in front of every service. Full write-up and incident postmortems (driver mismatches, mount misconfigurations, the usual) at [omrielcharizi.com](https://omrielcharizi.com).

## Looking for

DevOps, System Administration, NOC, or IT infrastructure: a team where I can build, break things in a controlled environment, and fix them down to the root cause.

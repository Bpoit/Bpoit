# Hey, I'm Chris 👋

**IT Professional | DevOps Enthusiast | Homelab Builder**

I work in IT at [Titan America](https://www.titanamerica.com) and spend my free time building out my homelab, learning DevOps, and gaming on Linux.

🌐 [b-clarke.com](https://b-clarke.com) &nbsp;|&nbsp; 🎮 [bpoit.tech](https://bpoit.tech)

---

## 🏠 ClarkesLAB — My Homelab

A full virtualized environment running Proxmox, self-hosted services, and a growing Kubernetes cluster.

### Compute

| Host | Hardware | Role | IP |
|------|----------|------|-----|
| **clab-pve01** | Intel i7-13700KF / 64GB RAM / Z690 | Primary Proxmox Hypervisor | `172.16.10.233` |
| **clab-gpu01** | AMD Ryzen 9 3950X / 32GB RAM / RTX 3080 | Gaming & GPU Workloads | `172.16.10.235` |
| **clab-k8-01** | Lenovo M80q / 16GB RAM | Kubernetes Control Plane | `172.16.10.234` |
| **K8s Workers** | 6x Lenovo M715q (planned) | Kubernetes Worker Nodes | — |

### Networking

| Device | Role |
|--------|------|
| **OPNsense** (Lenovo M720q) | Firewall / Router |
| **Cisco Catalyst 3850** | Managed Switch |
| **Synology DS920+** | NAS (~15TB) |

**VLANs:** `10` Home &nbsp;·&nbsp; `20` Servers &nbsp;·&nbsp; `30` IoT &nbsp;·&nbsp; `99` Management

### Virtualized Services (Proxmox LXC)

| VMID | Container | Purpose |
|------|-----------|---------|
| 105 | `homepage` | Dashboard |
| 106 | `pihole` | DNS Ad-Blocking & Local DNS |
| 107 | `mariadb` | Database Server |
| 108 | `nginxproxymanager` | Reverse Proxy & SSL |
| 109 | `b-clarke-wordpress` | [b-clarke.com](https://b-clarke.com) — IT Consulting Site |
| 110 | `cloudflare-tunnel` | Secure External Access |
| 111 | `ghost` | [goinggrey.info](https://goinggrey.info) — Ghost Blog |
| 112 | `hermes-agent` | AI Assistant (Hermes + Tailscale) |
| 113 | `bpoit-wordpress` | [bpoit.tech](https://bpoit.tech) — Gaming Community |

### Network Architecture

```
Internet → Cloudflare Tunnel (LXC 110) → Nginx Proxy Manager (LXC 108) → Backend Services
PiHole (LXC 106) handles local DNS resolution for all domains
Tailscale mesh VPN for remote access
```

---

## 🛠️ Tools & Technologies

**Infrastructure:** Proxmox VE · Docker · LXC · Kubernetes (learning)
**Networking:** OPNsense · Cisco IOS · VLANs · Cloudflare · Tailscale · Nginx Proxy Manager
**Platforms:** Linux (daily driver — Bazzite) · Windows
**Web:** WordPress · Ghost · Astra · GeneratePress
**IT Admin:** ServiceNow · Lansweeper · KACE · SmartDeploy · Citrix/Igel · Office 365
**AI/Automation:** Hermes Agent · Self-hosted AI workflows

---

## 🎯 What I'm Working On

- 🔧 Expanding my Kubernetes cluster with 6 worker nodes
- 📈 Building DevOps skills and automating my homelab
- 🎮 Running a gaming community at [bpoit.tech](https://bpoit.tech) with CubeCoders AMP
- 🤖 Self-hosting AI tools and building automation workflows

---

## 📫 Get In Touch

- 🌐 Website: [b-clarke.com](https://b-clarke.com)
- 📧 Email: b-clarke3@outlook.com

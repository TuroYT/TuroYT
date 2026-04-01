<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0D1117,50:6C63FF,100:00FF41&height=220&section=header&text=ROMAIN%20PINSOLLE&fontColor=00FF41&fontSize=50&fontAlignY=35&animation=fadeIn&desc=%E2%96%88%E2%96%88%20systems%20engineer%20%C2%B7%20selfhost%20maximalist%20%C2%B7%20saas%20builder%20%E2%96%88%E2%96%88&descSize=14&descAlignY=58&descAlign=50" width="100%"/>

<br/>

```
 ╔══════════════════════════════════════════════════════════════════╗
 ║  TERMINAL SESSION — node1.sheephost.fr                         ║
 ║  Last login: today from 64.xxx.xx.xx on pts/0                  ║
 ║  Uptime: since 2005 · Mass of infra deployed · 0 cloud bills   ║
 ╚══════════════════════════════════════════════════════════════════╝
```

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=00FF41)](https://linkedin.com/in/pinsolle)
[![Website](https://img.shields.io/badge/romain--pinsolle.fr-0D1117?style=for-the-badge&logo=googlechrome&logoColor=00FF41)](https://romain-pinsolle.fr)
[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=00FF41)](https://instagram.com/romain.pinsolle)
[![Discord](https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=00FF41)](https://discord.gg/turocestmoi)

</div>

<br/>

## `$ whoami`

```js
const romain = {
    name:       "Romain Pinsolle",
    aka:        "Turo",
    location:   "Pays Basque, France 🇫🇷",
    role:       "Alternant @ Safran Helicopter Engines",
    education:  "BUT Informatique",
    side_quest: "Building SaaS for local businesses",
    rides:      "Kawasaki Z400 🏍️",
    os:         "Arch Linux (btw)",
    uptime:     "99.7% — the 0.3% is motorcycle maintenance",
    mantra:     "If it can run on a server, it runs on MY server."
};
```

<br/>

## `$ cat /etc/stack.conf`

```yaml
# ─── APPLICATION LAYER ───────────────────────────────────────────
backend:
  framework:   NestJS
  language:    TypeScript (strict mode, obviously)
  orm:         [ TypeORM, Prisma ]
  databases:   [ PostgreSQL, SQL Server, MongoDB ]
  auth:        JWT / Passport / Google OAuth
  queues:      Redis + BullMQ
  payments:    Stripe
  monitoring:  Datadog APM

frontend:
  frameworks:  [ Ionic/Angular, React, Next.js ]
  styling:     [ Tailwind CSS, SCSS ]

mobile:
  stack:       Ionic Capacitor  # cross-platform, one codebase

# ─── INFRASTRUCTURE LAYER ────────────────────────────────────────
infra:
  hypervisor:  Proxmox VE         # Dell PowerEdge R730
  containers:  Docker Swarm
  deployment:  Dokploy
  reverse_proxy: Caddy            # automatic HTTPS, zero config
  object_storage: Garage S3       # self-hosted, s3-compatible
  automation:  n8n                # workflows > cron jobs
  ci_cd:       GitHub Actions
  security:    [ Semgrep, Zscaler ]
  dns:         Cloudflare
  domain:      sheephost.fr

# ─── PHILOSOPHY ──────────────────────────────────────────────────
philosophy:
  cloud_provider: "my closet"
  monthly_aws_bill: 0
  containers_running: "yes"
```

<div align="center">

<br/>

[![Tech Stack](https://skillicons.dev/icons?i=ts,nestjs,angular,react,nextjs,postgres,prisma,redis,docker,linux,arch,mongodb&theme=dark&perline=12)](https://skillicons.dev)

</div>

<br/>

## `$ ls -la ~/projects/`

```
drwxr-xr-x  romain romain  4096 Apr 01  snowshare/
drwxr-xr-x  romain romain  4096 Apr 01  armature/
drwxr-x---  romain romain  4096 Apr 01  lakartxela/        # 🔒
-rw-r--r--  romain romain   512 Apr 01  saas-ideas.encrypted
```

<table>
<tr>
<td width="50%" valign="top">

### 🗂️ [`snowshare`](https://github.com/TuroYT/snowshare)
> Self-hosted file & link sharing platform.  
> Next.js · Prisma · NextAuth  
> ⭐ 63 stars · GPL-3.0  
> *Because WeTransfer doesn't deserve your data.*

</td>
<td width="50%" valign="top">

### ⚙️ [`armature`](https://github.com/TuroYT/Armature)
> Opinionated NestJS boilerplate.  
> Prisma · JWT auth · RBAC · typed errors · i18n  
> Optional Redis/BullMQ · Stripe · Google OAuth  
> *The skeleton so you can ship the muscle.*

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🔐 `lakartxela`
> Digital loyalty card app for local businesses.  
> NestJS · Ionic/Angular · PostgreSQL  
> 🚧 In active development  
> *La carte de fidélité, version Neo-Basque Tech.*

</td>
<td width="50%" valign="top">

### 🧪 `saas-ideas.encrypted`
> ```
> gpg: decryption failed: No secret key
> ```
> *Nice try. Stay tuned.*

</td>
</tr>
</table>

<br/>

## `$ systemctl status homelab`

```
● homelab.service - Romain's Self-Hosted Empire
     Loaded: loaded (/etc/systemd/system/homelab.service; enabled)
     Active: active (running) since forever
   Main PID: 1337
     Memory: yes
      Tasks: too many

  ┌─────────────────────────────────────────────────────────────┐
  │                                                             │
  │   ┌──────────┐    ┌──────────┐    ┌──────────┐             │
  │   │ Proxmox  │───▶│  Docker  │───▶│ Dokploy  │             │
  │   │ (R730)   │    │  Swarm   │    │ (deploy) │             │
  │   └──────────┘    └──────────┘    └─────┬────┘             │
  │                                         │                  │
  │        ┌────────────────────────────────┬┘                  │
  │        ▼                ▼               ▼                  │
  │   ┌─────────┐    ┌──────────┐    ┌──────────┐             │
  │   │  Caddy   │    │ Garage   │    │   n8n    │             │
  │   │ (proxy)  │    │ S3       │    │ (auto)   │             │
  │   └─────────┘    └──────────┘    └──────────┘             │
  │                                                             │
  │   Services: Lakartxela · SnowShare · Etiqueo · Datadog · n8n │
  │   Domain:   *.sheephost.fr                                 │
  │   Status:   All systems nominal ✅                          │
  │                                                             │
  └─────────────────────────────────────────────────────────────┘
```

<br/>

## `$ neofetch`

<div align="center">

<img src="https://streak-stats.demolab.com?user=TuroYT&theme=highcontrast&hide_border=true&border_radius=12&ring=00FF41&fire=00FF41&currStreakLabel=00FF41&sideLabels=00FF41&dates=6C63FF" alt="GitHub Streak"/>

<br/>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=TuroYT&bg_color=0D1117&color=00FF41&line=6C63FF&point=00FF41&area_color=6C63FF&area=true&hide_border=true&custom_title=Contribution%20Graph&radius=12" width="95%" alt="Activity Graph"/>

<br/>

<img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=TuroYT&theme=github_dark" width="95%"/>

<br/>

![Profile Views](https://komarev.com/ghpvc/?username=TuroYT&style=for-the-badge&color=00FF41&label=PROFILE+VIEWS)

</div>

<br/>

## `$ fortune | cowsay`

```
 _____________________________________________
/ "Why do I have 47 Docker containers        \
| running on a server in my closet?"          |
|                                             |
| "Because AWS wanted €200/month and I have   |
|  a Dell PowerEdge and zero self-control."   |
|                                             |
| Anyway, je selfhost mes vaches aussi. 🐄    |
\ — Turo, probably                            /
 ---------------------------------------------
        \   ^__^
         \  (oo)\_______
            (__)\       )\/\
                ||----w |
                ||     ||
```

<br/>

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0D1117,50:6C63FF,100:00FF41&height=120&section=footer&animation=fadeIn" width="100%"/>

```
$ echo "Let's build something cool together"
> contact@romain-pinsolle.fr
```

```
/* Session closed. Connection to node1.sheephost.fr terminated. */
```

</div>

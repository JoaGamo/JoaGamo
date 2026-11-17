<div align="center">

# Joaquín Gamonal

### Information Systems Engineering Student · SysAdmin, SRE & Backend Developer

[![Blog](https://img.shields.io/badge/Blog-gamopc.com.ar-10172a?style=for-the-badge&logo=googlechrome&logoColor=white)](https://gamopc.com.ar)
[![Email](https://img.shields.io/badge/Email-joa%40gamopc.com.ar-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:joa@gamopc.com.ar)

![UNS](https://img.shields.io/badge/UNS-Information%20Systems%20Engineering-1e3a8a?style=flat-square)
![Argentina](https://img.shields.io/badge/Bahía%20Blanca-Argentina-74acdf?style=flat-square)

</div>

---

## About me

4th-year Information Systems Engineering student at **Universidad Nacional del Sur (UNS)**.

I run bare-metal servers, build distributed storage, write performance-sensitive backends and self-host LLM infrastructure on my own hardware. I'm looking for a supervised internship (PPS) in **DevOps, SRE or Platform Engineering**.

I write about my projects on **[gamopc.com.ar](https://gamopc.com.ar)**, and each repo explains its own design choices.

---

## Storage (my strongest area)

| Level | Technologies |
|---|---|
| **Deep experience** | Ceph · MooseFS · ZFS · bcachefs |
| **Worked with** | Btrfs · XFS · ext4 · DRBD · bcache |

![Ceph](https://img.shields.io/badge/Ceph-E95420?style=for-the-badge&logo=ceph&logoColor=white)
![MooseFS](https://img.shields.io/badge/MooseFS-005B9A?style=for-the-badge)
![ZFS](https://img.shields.io/badge/ZFS-053641?style=for-the-badge)
![bcachefs](https://img.shields.io/badge/bcachefs-2C2C2C?style=for-the-badge)

Writing on this:
- [Why I moved from Ceph to MooseFS](https://gamopc.com.ar/moosefs-and-you/): ~3 years of Ceph, and a comparison of distributed filesystems
- [bcachefs is all you need](https://gamopc.com.ar/bcachefs-is-all-you-need/): collapsing a 6+ node MooseFS cluster into a single bcachefs + NFS NAS to cut power consumption
- [Modding a GPU mining chassis into a hybrid NAS](https://gamopc.com.ar/converting-a-gpu-mining-chassis-to-a-ssd-h-nas-server/): the hardware side of that NAS

---

## Homelab & infrastructure

![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Proxmox](https://img.shields.io/badge/Proxmox_VE-E57000?style=for-the-badge&logo=proxmox&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![OPNsense](https://img.shields.io/badge/OPNsense-894C24?style=for-the-badge&logo=opnsense&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white)

LXC · QEMU/KVM · FFmpeg · Ansible · Netbird

Writing on this:
- [Gamopelis](https://gamopc.com.ar/gamopelis-my-distributed-self-hosted-movie-system-built-with-jellyfin-and-remote-ffmpeg/): distributed, self-hosted streaming built on Jellyfin and remote FFmpeg
- [Meilisearch for Jellyfin search](https://gamopc.com.ar/meilisearch-improving-jellyfin-search-results-and-speed-by-999/): fixing missing search results and speeding up search
- [Nginx Proxy Manager response buffering](https://gamopc.com.ar/your-nginx-proxy-mancould-be-bottlenecking-your-services/): tracking down a latency issue on small Jellyfin requests
- [Self-hosting Netbird with NPM and Zitadel](https://gamopc.com.ar/self-hosting-netbird-with-npm-and-zitadel/)
- [Games on Whales](https://gamopc.com.ar/games-on-whales-have-you-ever-wanted-to-host-your-own-cloud-gaming-server/): cloud gaming in containers

---

## AI & LLM infrastructure

I've been in generative AI since the early days (ComfyUI in its early era), and I now focus on **serving and integrating models on my own hardware**.

| Layer | Experience |
|---|---|
| Inference serving | vLLM · Aphrodite Engine · GPUStack · Ollama |
| Image generation | ComfyUI |
| Frontends / orchestration | Open WebUI · FastAPI backends |
| Applications | RAG tutor for 400+ students ([Physics I](https://github.com/JoaGamo/REPO)) |

<details>
<summary>Also tried / evaluated</summary>

<!-- Add the long tail here: llama.cpp, etc. Names only. -->

</details>

---

## Languages & backend

![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white)
![C](https://img.shields.io/badge/C-00599C?style=flat-square&logo=c&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Lua](https://img.shields.io/badge/Lua-2C2D72?style=flat-square&logo=lua&logoColor=white)

PostgreSQL · Redis · FastAPI · Next.js · Astro · Drizzle ORM · Prolog

---

## Projects

| Project | What it is | Links |
|---|---|---|
| **Physics I AI Agent** | RAG-based virtual tutor for 400+ UNS students. FastAPI, SymPy, Open WebUI, local LLMs. | [Repo](https://github.com/JoaGamo/REPO) |
| **ESP32 Homelab Telemetry** | Physical disk I/O monitor on an ESP32-C3 with a MAX7219 LED matrix. C (ESP-IDF), SPI. | [Repo](https://github.com/JoaGamo/REPO) |
| **RunConnect** | Real-time sports tracking platform. PostgreSQL, PostGIS, Drizzle ORM, Next.js. | [Repo](https://github.com/JoaGamo/REPO) |
| **GamoBots** | Telemetry and audio Discord bots. PostgreSQL, Python, Lavalink. | [Repo](https://github.com/JoaGamo/REPO) |
| **AeroGestión UNS** | Airline management system (Project Leader, PSS course). | [Repo](https://github.com/JoaGamo/REPO) |

---

## GitHub stats

<div align="center">

[![GitHub Stats](https://github-stats-extended.vercel.app/api?username=JoaGamo&include_all_commits=true&theme=midnight-purple)](https://github.com/JoaGamo)

</div>

---

<div align="center">

### Building infrastructure and reliable systems from the ground up.

</div>

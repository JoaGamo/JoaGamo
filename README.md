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

## Virtualization & operating systems

I know QEMU/KVM well, mostly from running a cloud gaming cluster at home, basically a small GeForce Now on a Proxmox cluster. Getting Windows guests to work properly meant going below Proxmox: I recompiled my own edk2 firmware and a custom build of QEMU, spoofed CPUID, SMBIOS and ACPI so software that refuses to run in a VM would work, and set up VFIO GPU passthrough to share GPUs between several guests. Then came the usual tuning for low-latency streaming, like CPU pinning and hugepages.

I started this as a teenager and learned most of what I know about how operating systems work by breaking things there.

I also wrote about a container-based take on the same idea: [Games on Whales](https://gamopc.com.ar/games-on-whales-have-you-ever-wanted-to-host-your-own-cloud-gaming-server/).

---

## AI & LLM infrastructure

I've been in generative AI since the early days (ComfyUI in its early era), and I now focus on **serving, routing and integrating models on my own hardware**. I've run most of the self-hosted LLM ecosystem, so the table below is grouped by layer.

| Layer | Hands-on experience |
|---|---|
| **Inference serving** | vLLM · llama.cpp · SGLang · TensorRT-LLM · Aphrodite Engine · ExLlamaV2/V3 (TabbyAPI) · KoboldCpp · Ollama · Lemonade Server · llama-swap |
| **Multi-GPU & clusters** | Ray · GPUStack · llama.cpp RPC · exo · Petals |
| **Gateways & routing** | LiteLLM · Bifrost · OpenRouter |
| **Quantization & fine-tuning** | Unsloth · bitsandbytes · GGUF · GPTQ · AWQ · INT4 |
| **RAG & search** | LlamaIndex · Qdrant · Chroma · Meilisearch |
| **Multimodal** | LLaVA · Qwen-VL · Florence-2 |
| **Image & video generation** | ComfyUI · Automatic1111 · Forge · Fooocus · Stable Diffusion · Flux · Wan · HunyuanVideo · Kohya (LoRA training) |
| **Speech** | faster-whisper · whisper.cpp · WhisperX · Piper · Coqui/XTTS · Kokoro · Parakeet |
| **Frontends & orchestration** | Open WebUI · SillyTavern · LibreChat · AnythingLLM · Flowise · Langflow |
| **Agents & automation** | n8n · Node-RED · Aider · Kilo Code |

**Applications built on top of this:** a RAG-based virtual tutor for 400+ UNS students, [[See here]](https://agente.fisica.uns.edu.ar)

### Observability

Grafana · Prometheus · InfluxDB (v2 and v3) · currently exploring the VictoriaMetrics stack.

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
| **Physics I AI Agent** | RAG-based virtual tutor for 400+ UNS students. FastAPI, SymPy, custom WebUI, local LLMs and local physics calculation. | [Website](https://agente.fisica.uns.edu.ar) |
| **ESP32 Homelab Telemetry** | Physical disk I/O monitor on an ESP32-C3 with a MAX7219 LED matrix. C (ESP-IDF), SPI. | Private |
| **RunConnect** | Real-time sports tracking platform. PostgreSQL, PostGIS, Drizzle ORM, Next.js. | [Repo](https://github.com/Sofiacosta2024/RunConnect) |
| **GamoBots** | Telemetry and audio Discord bots. PostgreSQL, Python, Lavalink. | [GamoStats](https://github.com/JoaGamo/GamoStats) (the rest is private) |
| **Farmacia UNS** | Pharmacy management system (Project Co-Leader, PSS course). | [Repo](https://github.com/homero-six-seven/farmaciauns) |

---

## GitHub stats

<div align="center">

[![GitHub Stats](https://github-stats-extended.vercel.app/api?username=JoaGamo&include_all_commits=true&theme=midnight-purple)](https://github.com/JoaGamo)

</div>

---

<div align="center">

### Building infrastructure and reliable systems from the ground up.

</div>

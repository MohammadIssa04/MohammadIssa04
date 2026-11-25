<h1 align="center">Hi, I'm Mohammad Issa</h1>

<p align="center">
  I build things that real people use every day: apps for my family's store, my car, my TV and my home.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white" alt="Kotlin">
  <img src="https://img.shields.io/badge/Jetpack%20Compose-4285F4?style=flat-square&logo=jetpackcompose&logoColor=white" alt="Jetpack Compose">
  <img src="https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white" alt="Java">
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" alt="FastAPI">
  <img src="https://img.shields.io/badge/Raspberry%20Pi-A22846?style=flat-square&logo=raspberrypi&logoColor=white" alt="Raspberry Pi">
  <img src="https://img.shields.io/badge/Home%20Assistant-18BCF2?style=flat-square&logo=homeassistant&logoColor=white" alt="Home Assistant">
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker">
  <img src="https://img.shields.io/badge/Proxmox-E57000?style=flat-square&logo=proxmox&logoColor=white" alt="Proxmox">
</p>

---

## Projects

| Project | What it is |
|---|---|
| **[smart-store-screen](https://github.com/MohammadIssa04/smart-store-screen)** | AI-made video ads, store music and price labels for my dad's grocery store. One phone app, one Raspberry Pi, running in a real store every day. |
| **[issa-music](https://github.com/MohammadIssa04/issa-music)** | My own music app for the phone, my BMW's iDrive screen and the TV, streaming from my own server. |
| **[homelab](https://github.com/MohammadIssa04/homelab)** | My self-hosted home server on Proxmox: about 20 services for media, the smart home, files, security and monitoring. |
| **[tv-home](https://github.com/MohammadIssa04/tv-home)** | A custom Android TV home screen with a clock, weather, a now-playing widget and synced lyrics. |

## Home lab

One box under the desk runs almost everything at home, about 20 services, each in its own container. The full write-up is in **[homelab](https://github.com/MohammadIssa04/homelab)**.

**Hardware**

| Part | Spec |
|---|---|
| Hypervisor | Proxmox VE 9 |
| CPU | AMD Ryzen 5 3600 (6 cores / 12 threads) |
| RAM | 32 GB |
| GPU | NVIDIA GTX 1660 Ti (video transcoding and AI voice) |
| Storage | SSD for containers + a 10 TB disk for media and backups |
| Store | A Raspberry Pi 4 in my dad's grocery store |

**What I host**

| Area | Services |
|---|---|
| Media | Jellyfin with hardware transcoding, the *arr stack, my own music server for Issa Music |
| Smart home | Home Assistant, n8n automations |
| Cloud and files | Nextcloud, Syncthing |
| Security | Vaultwarden, Pocket ID (passkey sign-in), CrowdSec, AdGuard Home, a honeypot |
| Monitoring | Uptime Kuma, Beszel, a Homepage dashboard, my own ntfy push server, self-healing scripts |
| AI | Local text-to-speech, an AI agent that helps run the server |
| Offline | Wikipedia offline with Kiwix (English and Swedish) |

No ports are forwarded on the router: I reach it from outside over a private VPN. Backups run every night, with an encrypted copy off-site.

## How I like to build

- **Built for the real user.** If my dad has to call me, the app isn't done.
- **Measure first.** Small hardware goes far when you optimise what actually matters.
- **Never lose anything.** Backups, health checks and "archive, don't delete".

# NERD – Networked Environment for Resource Deployment
Welcome to my HomeLab Repository! I recently rescued an old Dell E10S from a skip, along with a Lenovo x3650 M4 (which is currently just a very heavy paperweight). 
While the Lenovo isn't operational yet - and honestly a bit too loud for my setup anyways - the Dell has become my main testing platform.

## 🖥️ Hardware

| Device          | CPU                        | RAM                 | Storage                              | Purpose                |
|-----------------|----------------------------|---------------------|--------------------------------------|------------------------|
| Dell E10S       | i3-2120 CPU @ 3.3GHz       | 12GB DDR3 1333 MT/s | 500GB HDD                            | Proxmox Host           |
| Lenovo x3650 M4 | 2x Xeon E5-2620 v2 @2.1GHz | 96GB DDR3 1600 MHz  | 4x 1.2TB SAS + 12x 6GB SAS FRU 300GB | Future Storage Server? |

## 🏗️ Running VMs/Containers
```shell
.
└── 🖥️ Dell E10S - Proxmox VE 8.4.0                                # Main Proxmox Server
    ├── 💽 Debian 12.11.0 - 1 sockets, 2 cores, 8GB RAM, 32GB HDD  # Lightweight Linux OS
    │   └── 📂 Paper 1.21.8-8                                      # Minecraft Server
    └── 💽 Ubuntu 24.04.2 - 1 sockets, 2 cores, 4GB RAM, 32GB HDD  # Docker Container Server
        ├── 📂 Homarr 1.30.0                                       # Main HomeLab Dashboard
        └── 📂 Home Assistant 2025.7.2                             # Home Automation
```

## 🛠️ Planned Upgrades / TODO

- [ ] Add dual M.2 PCIe SSD card for faster storage
- [ ] Upgrade RAM to 16–32GB
- [ ] Deploy TrueNAS VM for network storage
- [ ] Enable remote backups to external drive
- [ ] Add HTTPS via reverse proxy for Homarr & Home Assistant

## 📦 Software & Tools

- Proxmox VE 8.4.0 (Main hypervisor)
- Docker (via Ubuntu VM)
- Homarr (dashboard for service links)
- Home Assistant (local automation)
- PaperMC (lightweight Minecraft server)

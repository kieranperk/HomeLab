# NERD – Networked Environment for Resource Deployment
Welcome to my HomeLab Repository! I rescued a few old systems from my work's skip after their infrastructure change. These systems consisted of a Dell D11S Desktop PC, a Dell E10S 1U Server along with a Lenovo x3650 M4 (which is currently just a very heavy paperweight due to myself not being able to dedicate the time to make it operational yet).

## 🖥️ Hardware

| Device          | CPU                        | RAM                 | Storage                              | Purpose                |
|-----------------|----------------------------|---------------------|--------------------------------------|------------------------|
| Dell D11S       | i7-7700 CPU @ 3.60GHz      | 8GB DDR4 2400MHz    | 500GB HDD                            | Proxmox Host           |
| Dell E10S       | i3-2120 CPU @ 3.3GHz       | 12GB DDR3 1333 MT/s | 500GB HDD                            | ---                    |
| Lenovo x3650 M4 | 2x Xeon E5-2620 v2 @2.1GHz | 96GB DDR3 1600 MHz  | 4x 1.2TB SAS + 12x 6GB SAS FRU 300GB | ---                    |

## 🏗️ Running VMs/Containers
```shell
.
└── 🖥️ Dell D11S - Proxmox VE 9.2.2                                 # Main Proxmox Server
    └── 💽 Home Assistant OS 2026.8.2 - 2 cores, 4GB RAM, 32GB HDD  # Docker Container Server
        ├── 📂 AdGuard Home 6.2.0                                   # Network-wide Adblocker via DNS
        ├── 📂 Mosquitto Broker 7.1.0                               # MQTT Protocol Experimentation
        └── 📂 Tailscale 0.28.1                                     # Tunneled VPN for Connecting Externally
```
The reason why all my services are currently being run on the Dell D11S is partially due to the overall power draw of the system being quite low and the performance being better than the other systems, but mainly due to the noise. My HomeLab is currently being stored inside of my bedroom, therefore the systems have to be quiet enough to stay online whilst I sleep.

## 🛠️ Planned Upgrades / TODO

- [ ] 

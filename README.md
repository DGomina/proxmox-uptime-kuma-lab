# proxmox-uptime-kuma-lab
Created my own VM in VirtualBox running Proxmox VE, then spun up Uptime Kuma in a Linux container to track endpoint uptime (set up a ping monitor to Google DNS to test it).

Installed Proxmox VE inside a VirtualBox VM and deployed Uptime Kuma in a Linux container to monitor endpoint uptime (including ping checks to Google DNS).

Fixes during setup:
- Configured static IP (10.0.2.16) and port forwarding (port 3001) to resolve VirtualBox NAT routing conflicts.
- Enabled container nesting and adjusted AppArmor permissions so Uptime Kuma would run inside the container.

# The Homelab Initiative
Hardware:\n
           Odin - R7 5700g, 32GB, 1TB SSD\n
           R730xd - 2x E5-2620v3, 32GB, 2TB SSD\n
           R630 - 1x E5-2620v3, 12GB, 300GB HDD\n

Services:\n
           [Proxmox](https://www.proxmox.com/en/)\n
           [TrueNAS Scale](https://www.truenas.com/truenas-scale/)\n
           [Rancher](https://rancher.com/)\n
           [Terraform](https://www.terraform.io/)\n
           [Ansible](https://www.ansible.com/)\n
           [Puppet](https://puppet.com/)\n
           [Veeam](https://www.veeam.com/)\n
           [Prometheus](https://prometheus.io/)\n
           [Traefik](https://traefik.io/)\n
           [NGINX](https://www.nginx.com/)\n
           [Grafana](https://grafana.com/)\n
           [Pterodactyl](https://pterodactyl.io/)\n
           [Bitwarden](https://bitwarden.com/)\n
           [Pi-hole](https://pi-hole.net/)\n
           [Active Directory](https://docs.microsoft.com/en-us/windows-server/identity/ad-ds/get-started/virtual-dc/active-directory-domain-services-overview)\n
           [Tdarr](https://tdarr.io/)\n
           [Kodi](https://kodi.tv/)\n
           [Jellyfin](https://jellyfin.org/)\n
           [Nextcloud](https://nextcloud.com/)\n
           [Keycloak](https://www.keycloak.org/)\n

Storage:\n
           12 HDDs used for mass storage in RAID6 or RAID10.\n
           8 SSDs in raid 5/10 for quick read/write storage such as databases.\n
           Each server has 2 internal SSDs in RAID1 for redundancy that the OSes and VMs are stored on.\n

3-2-1 backup philosophy:\n
           3 copies of all data that I want to keep\n
           2 on-prem copies, 1 on the SSDs, 1 on the HDDs\n
           1 Copy in the cloud (Wasabi or Backblaze)\n
           Any exceptions to this policy should be documented and justified\n
           Initial exceptions: Movies/Mass Media\n
           Special Cases: Personal media (HDD copy and cloud copy)

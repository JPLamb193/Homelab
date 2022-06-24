# The Homelab Initiative
Hardware:
           Odin - R7 5700g, 32GB, 1TB SSD
           R730xd - 2x E5-2620v3, 32GB, 2TB SSD
           R630 - 1x E5-2620v3, 12GB, 300GB HDD

Services:
           [Proxmox](https://www.proxmox.com/en/)
           [TrueNAS Scale](https://www.truenas.com/truenas-scale/)
           [Rancher](https://rancher.com/)
           [Terraform](https://www.terraform.io/)
           [Ansible](https://www.ansible.com/)
           [Puppet](https://puppet.com/)
           [Veeam](https://www.veeam.com/)
           [Prometheus](https://prometheus.io/)
           [Traefik](https://traefik.io/)
           [NGINX](https://www.nginx.com/)
           [Grafana](https://grafana.com/)
           [Pterodactyl](https://pterodactyl.io/)
           [Bitwarden](https://bitwarden.com/)
           [Pi-hole](https://pi-hole.net/)
           [Active Directory](https://docs.microsoft.com/en-us/windows-server/identity/ad-ds/get-started/virtual-dc/active-directory-domain-services-overview)
           [Tdarr](https://tdarr.io/)
           [Kodi](https://kodi.tv/)
           [Jellyfin](https://jellyfin.org/)
           [Nextcloud](https://nextcloud.com/)
           [Keycloak](https://www.keycloak.org/)

Storage:
           12 HDDs used for mass storage in RAID6 or RAID10.
           8 SSDs in raid 5/10 for quick read/write storage such as databases.
           Each server has 2 internal SSDs in RAID1 for redundancy that the OSes and VMs are stored on.

           3-2-1 backup philosophy:
           3 copies of all data that I want to keep
           2 on-prem copies, 1 on the SSDs, 1 on the HDDs
           1 Copy in the cloud (Wasabi or Backblaze)
           Any exceptions to this policy should be documented and justified
           Initial exceptions: Movies/Mass Media

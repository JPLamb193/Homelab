# Homelab Documentation

## Hardware:  
Zeus - Supermicro H11, ADM Epyc 32 core, 64GB ECC RAM, 1.6TB Intel DC P3600, 960GB Samsung PM883  
Poseidon - ASRock B550M, Ryzen 5700, 64GB ECC RAM, 1.6TB Intel DC P3600, 960GB Samsung PM883  
Hades - ASRock B550M, Ryzen 5600x, 64GB ECC RAM, 1.6TB Intel DC P3600, 960GB Samsung PM883  
Hera -  


## Services:  
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
[Authentik](https://goauthentik.io/)  

## Storage:  
All 5 main nodes are hyperconvered, running Ceph for storage. Each node has 1, 1TB SSD that is housing the OS, and a 1.6TB NVMe SSD that is being used in a Ceph pool to house VMs, containers, etc.  

A 0 replication Ceph pool with a few spinning rust drives will house the mass media from sonarr, radarr, etc.  

Separate storage pool for backups WIP.  

### 3-2-1 backup philosophy:  
3 copies of all data that I want to keep  
2 on-prem copies- On-Prem copies covered by Ceph, and the backup(s)  
1 Copy in the cloud (Wasabi or Backblaze) - WIP, may be too expensive to be worth doing for a small scale home setup like this.  
Any exceptions to this policy should be documented and justified  
Initial exceptions: Movies/Mass Media  
Special Cases: Personal media (HDD copy and cloud copy)  

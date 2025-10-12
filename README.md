# aruzi
Minimal headless server for direct music/movies streaming + VPN

## Design*
_(armbian on a Libre Computer Renegade ROC-RK3328-CC running multiple docker containers)_

**dashboard:** Glance (quick look at Aruzi's status)

 **music:** Navidrome + mpv (music streaming and playing capabilities)
 
 **vpn:** Tailscale (secure vpn to access the servers other devices)
 
 **books:** Kavita (book server)
 
 **movies:** Plex (movies/music server)

 **torrent:** qBittorrent (web interface for downloading torrents)

 **metrics:** Grafana (access to CPU, RAM and other resources metrics)

 **proxy:** Caddy (URL redirect)
 
 **watchtower:** containers updater

*This design assummes a DAC will be plugged for Hi-Res Music streaming. Also, that there will be no transcoding at all, if that's the case, this setup barely consumes power. Finally, an external drive is required for media storage (in my case, a 2TB SATA SSD connected to a USB-to-SATA adapter), and a decent microSD is recommended to flash and run the OS.

 ## Software

- **rsync:** for file uploading
- **docker:** for containerization 



# aruzi
Minimal headless server for software independence

## Design*
_(armbian on a Libre Computer Renegade ROC-RK3328-CC running multiple docker containers)_

**dashboard:** Glance (quick look at Aruzi's status)

 **music:** Navidrome + mpv (music streaming and playing capabilities)
 
 **vpn:** headscale (secure vpn to access to content from other devices)
 
 **books:** Kavita (book server)
 
 **movies:** Plex (movies/music server)

 **torrent:** qBittorrent (web interface for downloading torrents)

 **paswords:** Vaultwarden (password manager)

 **blog:** Hugo

 **metrics:** Grafana (access to CPU, RAM and other resources metrics)

 **proxy:** Caddy (URL redirect)
 
 **watchtower:** containers updater

*This design assummes a DAC will be plugged for Hi-Res Music streaming. Also, that there will be no transcoding at all, if that's the case, this setup barely consumes power. Finally, an external drive is required for media storage (in my case, a 2TB SATA SSD connected to a USB-to-SATA adapter) and to flash/run the OS.

 ## Software

- **rsync:** for file uploading
- **docker:** for containerization

 ## Other capabilities

 - Automatic generation of a 320kbps copy for hi-res albums.



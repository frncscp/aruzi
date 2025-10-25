# aruzi
Minimal headless server for software independence

## Design*
_(armbian on a Libre Computer Renegade ROC-RK3328-CC running multiple docker containers)_

**dashboard:** Glance (quick look at Aruzi's status)

 **music:** Navidrome + mpv (music streaming and playing capabilities)
 
 **vpn:** headscale + headplane (secure vpn to access to content from other devices)
 
 **docs:** paperless-ngx (docs server)
 
 **movies:** Plex (movies/music server)

 **paswords:** Vaultwarden (password manager)

 **metrics:** Grafana (access to CPU, RAM and other resources metrics)

 **proxy:** Caddy (URL redirect)

 **share** snapdrop (remote file transfer)

 **manager** Portainer (container manager)
 
 **watchtower:** containers updater

*This design assummes a DAC will be plugged for Hi-Res Music streaming. Also, that there will be no transcoding at all, if that's the case, this setup barely consumes power. Finally, an external drive is required for media storage (in my case, a 2TB SATA SSD connected to a USB-to-SATA adapter) and to flash/run the OS.

 ## Other capabilities

 - Automatic generation of a 320kbps copy for hi-res albums.



```
   _____                     .__ 
  /  _  \_______ __ _________|__|
 /  /_\  \_  __ \  |  \___   /  |
/    |    \  | \/  |  //    /|  |
\____|__  /__|  |____//_____ \__|
        \/                  \/   
```

Minimal headless server for software independence

## Design*
_(NixOS on a Libre Computer Renegade ROC-RK3328-CC running multiple docker containers)_

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

## Installation

- Get latest NixOS Minimal Installation and proceed with manual installation (all details [here](https://nixos.wiki/wiki/NixOS_Installation_Guide))
- Add git and docker to your NixOS config
- Clone this repo wherever you like
- Add `source path/to/aruzi/core/bash` to your .bashrc file
- Create your core.env file based on the example provided
- Run this command `aruzi` like if it were docker compose (aruzi up, aruzi down, etc), assuming the repo was cloned at $HOME

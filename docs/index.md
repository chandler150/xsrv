# xsrv

[![](https://gitlab.com/nodiscc/xsrv/badges/master/pipeline.svg)](https://gitlab.com/nodiscc/xsrv/-/pipelines)
[![](https://bestpractices.coreinfrastructure.org/projects/3647/badge)](https://bestpractices.coreinfrastructure.org/projects/3647)

**Install and manage self-hosted services/applications on your own server(s).**

`xsrv` provides:

- a [command-line tool](usage.html#command-line-usage) (wrapper around  [`ansible`](https://en.wikipedia.org/wiki/Ansible_%28software%29)) for simple deployments, maintenance and configuration
- a collection of ansible [roles](#roles) for various network services, web applications, system administration and infrastructure
- a base [playbook to setup a single server](installation/first-deployment.html) for personal use or small/medium teams


## Roles

- [common](roles/common) - base system components (SSH, upgrades, users, hostname, network, kernel, time...)
- [backup](roles/backup) - incremental backup service (local and remote backups)
- [monitoring](roles/monitoring) - monitoring, alerting and log agregation system (netdata, rsyslog, other tools)
- [apache](roles/apache) - Apache web server and PHP-FPM interpreter
- [homepage](role/homepage) - simple web server homepage
- [postgresql](roles/postgresql) - PostgreSQL database server
- [mariadb](roles/mariadb) - MariaDB (MySQL) database server
- [nextcloud](roles/nextcloud) - File hosting/sharing/synchronization/groupware/"private cloud"
- [tt_rss](roles/tt_rss) - Tiny Tiny RSS web feed reader
- [samba](roles/samba) - Cross-platform file and printer sharing service (SMB/CIFS)
- [shaarli](roles/shaarli) - personal, minimalist, super-fast bookmarking service
- [gitea](roles/gitea) - Lightweight self-hosted Git service/software forge
- [transmission](roles/transmission) - Bittorrent client/web interface/seedbox service
- [mumble](roles/mumble) - Low-latency voice-over-IP (VoIP) server
- [openldap](roles/openldap) - LDAP directory server and web administration tools
- [docker](roles/docker) - Docker container platform
- [rocketchat](roles/rocketchat) - Realtime web chat/communication platform


[![](https://screenshots.debian.net/screenshots/000/015/229/thumb.png)](roles/monitoring)
[![](https://i.imgur.com/PPVIb6V.png)](roles/nextcloud)
[![](https://i.imgur.com/UoKs3x1.png)](roles/tt_rss)
[![](https://i.imgur.com/8wEBRSG.png)](roles/shaarli)
[![](https://i.imgur.com/Rks90zV.png)](roles/gitea)
[![](https://i.imgur.com/blWO4LL.png)](roles/transmission)
[![](https://i.imgur.com/jYSU9zC.png)](roles/mumble)
[![](https://screenshots.debian.net/screenshots/000/006/946/thumb.png)](roles/openldap)
[![](https://i.imgur.com/OL7RZXb.png)](roles/rocketchat)
[![](https://i.imgur.com/3ZwPVQNs.png)](roles/homepage)


## Documentation

- [Installation](installation.md)
  - [Server preparation](installation/server-preparation.md)
  - [Controller preparation](installation/controller-preparation.md)
  - [First deployment](installation/first-deployment.md)
- [Usage](usage.md)
- [Maintenance](maintenance.md)
  - [Backups](maintenance/backups.md)
  - [Upgrading](maintenance/upgrading.md)
- [Advanced usage](advanced.md)
<<<<<<< HEAD
  - [Version control](advanced/version-control.md)
  - [Continuous deployment](advanced/continuous-deployment.md)
  - [Using as ansible collection](advanced/using-as-ansible-collection.md)
=======
>>>>>>> 436eb6b... doc: merge advanced usage subpages, merge maintenance subpages
- [Contributing](contributing.md)

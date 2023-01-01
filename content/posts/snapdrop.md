---
title: "Snapdrop"
date: 2023-01-01T13:20:27+08:00
draft: true
---

# Snapdrop Installation
---

```.yaml
---
version: "2.1"
services:
  snapdrop:
    image: lscr.io/linuxserver/snapdrop:latest
    container_name: snapdrop
    environment:
      - PUID=1000
      - PGID=1000
      - TZ=Europe/London
    #volumes:
    #  - <path to config>:/config
    ports:
      - 80:80
      - 443:443
    restart: unless-stopped
```

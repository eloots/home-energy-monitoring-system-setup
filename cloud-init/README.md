# `cloud-init` configuration files

## What do these configuration file do?

- Install `EMQX` MQTT Broker
- Install and configure Telegraf
- Install and configure InfluxDB v1.8
- Install Grafana server
- Install various utilities such as `fzf`
- Add a user `akkapi` with zsh as login shell + `oh-my-zsh` and fzf
  command history search
- Install `cloud-init` installation progress tracker. You need an
  RGB LED strip to use this (if you haven't you don;t get a visual 
  clue about the installation progress

### `smappee-2.yml`

- Verified on Raspberry Pi 4 Model B - 8GB
- Ubuntu 20.04 as OS (can be booted of SSD when a bootable SD is present)

#### Known issues

- The `cloud-init` progress tracker doesn't work on the latest HW version
  of a Raspberry Pi 4 Model B - 8GB. This may also be the case on other
  1, 2, and 4 GB boards

  The workaround is to use `smappee-2-ubuntu-22-04.yml`

### `smappee-2-ubuntu-22-04.yml`

- Verified on Raspberry Pi 4 Model B - 8GB
- Uses Ubuntu 22.04 as OS which can boot of an SSD attached to one of the
  USB-3 connectors


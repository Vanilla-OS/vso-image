# Vanilla OS VSO Image

Containerfile for building a Vanilla OS VSO image.

This image is based on top of [`vanillaos/pico`](https://github.com/Vanilla-OS/pico-image/pkgs/container/pico) and adds the systemd package to obtain a full systemd environment for VSO.

## Build

```bash
podman image build -t vanillaos/vso .
```

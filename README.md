# Vanilla OS VSO Image

Containerfile for building a Vanilla OS VSO image.

This image is based on top of [`vanillaos/pico`](https://github.com/Vanilla-OS/pico-image/pkgs/container/pico) and adds the systemd package to obtain a full systemd environment for VSO.

## Build

```bash
podman image build -t vanillaos/vso .
```

## Verify Image Build Provenance Attestation

All the image builds/pushes are attested for build provenance and integrity using the [attest-build-provenance](https://github.com/actions/attest-build-provenance) action. The attestations can be verified [here](https://github.com/Vanilla-OS/dev-image/attestations) or by having the latest version of [GitHub CLI](https://github.com/cli/cli/releases/latest) installed in your system. Then, execute the following command:

```sh
gh attestation verify oci://ghcr.io/vanilla-os/vso:main --owner Vanilla-OS
```

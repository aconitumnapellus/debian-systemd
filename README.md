# debian-systemd

Debian systemd container image to test with podman/molecule

To use it:
`podman pull ghcr.io/aconitumnapellus/debian-systemd:main`

To build it locally, clone the repository and build it using:

`podman build -t localhost/debian-systemd:bookworm .`

An example configuration for molecule is attached.
Make sure, when you initialize a molecule configuration, to remove the `create.yml` playbook, as it does not work with podman.

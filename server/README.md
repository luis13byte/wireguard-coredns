# Wireguard VPN server

## Requeriments

- Public ip or domain that accepts inbound traffic on port 51820.
- The host system must be debian based in order to share its respective kernel files with the container (/lib/modules).

# Instructions

Modify the docker-compose with the server data (public ip or domain) and if you want you can change the DNS server by modifying the PEERDNS variable, then start the container.

To see the configuration for a client connection go to the /config/peerX path in the container or use the mounted volume.

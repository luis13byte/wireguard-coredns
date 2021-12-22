# Wireguard VPN client (container)

The client mode of this container image is simply enabled by not setting the PEERS environment variable..

If you get IPv6-related errors in the log and the connection cannot be established, edit the AllowedIPs line in your peer/client wg0.conf to include only 0.0.0/0 and not ::/0; and restart the container.

## Requeriments

- The host system must be debian based in order to share its respective kernel files with the container (/lib/modules).

## Instructions

Modify the docker-compose with the server data and import the client configuration file in .disk/config/wg0.conf and start the container.

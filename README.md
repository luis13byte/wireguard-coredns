# wireguard-coredns
Configuration for deploy Wireguard server and client.

## Start the VPN server
Now you can start your WireGuard container with the following command and clients should be able to connect.
~~~
docker-compose up -d
~~~

## Add additional clients
If you want to add additional clients, you simply can increase the PEERS parameter in the docker-compose.yaml file. After changing this value you need to restart your docker container with the –force-recreate parameter.
~~~
docker-compose up -d --force-recreate
~~~

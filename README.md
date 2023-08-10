# chainweb-node-proxy
nginx config that can be used to place in front of a chainweb node to offer the endpoints from a single socket. eg for use with the chain-relay app

How to use:

- Install chainweb node
- Install nginx eg on debian derivatives: `apt install nginx libnginx-mod-http-headers-more-filter`
- Make sure the chainweb node p2p port is set to 8888 (or some port of your choice) and the interface to localhost -assuming nginx is installed on the same server as the node- in the node config.yaml and matches the P2P endpoint in proxy.txt
  
```
p2p:
  peer:
    interface: localhost
``` 

- put your valid certificate in place
- Copy proxy.txt to /etc/nginx/sites-available/default
- restart nginx

Questions or more info on https://discord.com/channels/502858632178958377/879895335512719400

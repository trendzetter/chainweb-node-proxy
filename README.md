# chainweb-node-proxy
nginx config that can be used to place in front of a chainweb node to offer the endpoints from a single socket. eg for use with the chain-relay app

How to use:

- Install chainweb node: https://github.com/Thanos420NoScope/node-setup
- Install nginx
- Make sure the chainweb node p2p port is set to 8888 (or some port of your choice) in /root/kda/config.yaml and matches the P2P endpoint in proxy.txt
- put your valid certificate in place
- Copy proxy.txt to /etc/nginx/sites-available/default
- restart nginx

Questions or more info on https://discord.com/channels/502858632178958377/879895335512719400

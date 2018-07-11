Description
=============

Start ngrok tunnels as a systemd service. All ngrok files place in /opt/ngrok..


Usage
============
1. Customize and copy `ngrok.service` to /etc/systemd/system/
2. Execute from root `systemctl enable ngrok.service`
3. Execute `systemctl daemon-reload` when the service file is changed


Example
============
1. Place authToken from ngrok-site to /opt/ngrok/ngrok.conf
2. Add proper config to `/opt/ngrok/ngrok.conf`.
   The `ngrok.conf.example` can be a start. See https://ngrok.com/docs#config for details of writing config files
3. Execute `systemctl enable ngrok.service`

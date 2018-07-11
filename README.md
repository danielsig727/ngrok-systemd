Description
=============

Start ngrok tunnels as a systemd service. All ngrok files place in /opt/ngrok..


Usage
============
1. Customize and copy `ngrok.service` to /etc/systemd/system/
2. Execute from root `systemctl enable ngrok.service`
3. Execute 'systemctl daemon-reload'


Example
============
1. Place authToken from ngrok-site to /opt/ngrok/ngrok.conf
2. Add tunell description to /opt/ngrok/ngrok.conf
	tunnels:
	  openvpn:
    	    remote_port: 51194
            proto:
             tcp: 1194
	
3. execute `systemctl enable ngrok.service`



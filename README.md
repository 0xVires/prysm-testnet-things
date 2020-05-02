# prysm-testnet-things
Some scripts and services for the testnet

# creating a systemd service for the beacon node
This will automatically restart the prysm beacon node on failure

1) **Adjust the prysmbeacon.service file accordingly (User, ExecStart)**
2) Save it in /etc/systemd/system/prysmbeacon.service
3) Start service with `sudo systemctl start prysmbeacon`
4) Watch live output with `journalctl -f -u prysmbeacon` - or just `journalctl -u prysmbeacon` to view logs
5) Show service status: `systemctl status prysmbeacon` or `systemctl show prysmbeacon`

# ETH2 Prysm Dashboard

Import the ETH2-prysm-dashboard.json file into grafana.

Credits to Guillaume Miralles for the original dashboard and the instructions for the setup: https://gist.github.com/GuillaumeMiralles/ef8617bd8cb245f25a1e384613ec1303 

![ETH2-Prysm-Dashboard](https://github.com/ppunktw/prysm-testnet-things/blob/master/eth2-prysm-dashboard.PNG)

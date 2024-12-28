# dummy-systemd-service-
Firstly, install dummy.sh into your system.
```
sudo cp dummy.sh /usr/bin/dummy.sh
```
Secondly, install dummy.service into your system.
```
sudo cp dummy.service /etc/systemd/system/dummy.service
```
After installing service:
```
sudo systemctl daemon-reload
sudo systemctl enable dummy.service
sudo systemctl is-enabled dummy.service
```
If you see enabled output you are good to go.
See details with:
```
sudo systemctl status dummy
```
# Interacting with the service
```
sudo systemctl start dummy
sudo systemctl stop dummy
sudo systemctl enable dummy
sudo systemctl disable dummy
sudo systemctl status dummy
```
# Check the logs
```
sudo journalctl -u dummy -f
```
This project is part of [roadmap.sh](https://roadmap.sh/projects/dummy-systemd-service) projects.

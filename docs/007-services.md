# Services and Systemd

The project uses systemd to manage Linux services.

### Common operations:

```
systemctl status <service>
systemctl start <service>
systemctl stop <service>
systemctl restart <service>
systemctl enable <service>
systemctl disable <service>

```
A custom systemd service is also implemented:

```
configs/linux-lab.service

```
The service demonstrates:
- Service creation
- Service startup
- Automatic restart
- Service dependencies
- Service logging
- Boot-time service activation

### Example:

```
sudo systemctl daemon-reload
sudo systemctl start linux-lab
sudo systemctl enable linux-lab

```

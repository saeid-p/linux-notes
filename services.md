# Linux Services

To see a list of running services on your Ubuntu system, you can use the systemctl command.
```
systemctl list-units --type=service

# Filter by service status.
systemctl list-units --type=service --state=active
```

To view more detailed information about a specific service, you can use the status command, for example:
```
systemctl status service-name
```

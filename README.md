# .Net Systemd Unit

This repository contains the configuration file for a systemd unit used to host a .NET application on a Linux distribution. Systemd is an init system that provides a standard process for controlling what programs run when a Linux system boots up, making it ideal for managing and maintaining long-running applications, like those built in .NET.

## Overview: 
This configuration file simplifies the process of deploying and managing .NET applications on Linux servers. It ensures that your .NET application is started as a service, restarted automatically if it crashes, and controlled via standard systemd commands (e.g., start, stop, restart, enable, and disable).

## Usage :
Rename ServiceName and Path in file.
</br>

Add The File To :
</br>
`/etc/systemd/system/myapp.service`

Reload Systemd:
```bash
sudo systemctl daemon-reload
```

Enable and Start The Service:
```bash
sudo systemctl enable myapp.service
sudo systemctl start myapp.service
```

Check the Status:
```bash
sudo systemctl status myapp.service
```
Logs and Troubleshooting:
```bash
journalctl -u myapp.service -e
```

Restart the service:
```bash
sudo systemctl restart myapp.service
```



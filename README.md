This is config file for systemd unit of a .net application used for hosting .net application on a linux distribution.

Rename ServiceName and Path in file.
</br>

Add The File To :
</br>
/etc/systemd/system/myapp.service

Reload Systemd:
</br>
`sudo systemctl daemon-reload`

Enable and Start The Service:
</br>
`sudo systemctl enable myapp.service`
</br>
`sudo systemctl start myapp.service`

Check the Status:
</br>
`sudo systemctl status myapp.service`

Logs and Troubleshooting:
</br>
`journalctl -u myapp.service -e`

Restart the service:
</br>
`sudo systemctl restart myapp.service`



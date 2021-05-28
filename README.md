# ndi-discovery.service

*N.B: In the Windows version of the SDK the process is called ndi-discovery-service, in the Linux version it's called ndi-directory-service for some reason. I choose to leave the name as is on the binary but name the service ndi-discovery.service.*
## Installation
1. Copy the NDI Discovery binary to ```/usr/local/bin/ndi-discovery-service```
2. Copy the systemd unit file from the git repo to ```/lib/systemd/system/ndi-discovery.service```
3. Refresh systemd with the command ```sudo systemctl daemon-reload```
4. Enable autostart of the service by running ```sudo systemctl enable ndi-discovery.service```
5. Start the service by running ```sudo systemctl start ndi-discovery.service```

To check status of the process, run ```sudo systemctl status ndi-discovery.service```
# Nagios kernel checker

This Nagios plugin checks whether the latest installed kernel is running or whether a reboot is required.

This check, to be called via NRPE, runs on RHEL based distributions.

## Installation

copy the check_kernelreboot file to /usr/lib64/nagios/plugins on the client

Add the following line to the /etc/nagios/nrpe.cfg file

```conf
command[check_kernelreboot]=$plugindir/check_kernelreboot
```


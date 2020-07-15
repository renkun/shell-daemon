# Shell-Daemon

Monitor shell scripts running, restart them once they're daed.

## How to use

All scripts can be configured in the shell-daemon.cnf file. 

```ini
daemon[0]="ping www.baidu.com"
daemon[1]="date > /tmp/date.log"
daemon[2]="node --version"
```

Also the checking time can be configured as below by seconds:

```ini
interval=10 
```

The scripts can be put to /etc/init.d, and set as running service

## NOTES!!!

SERVICE START MODE SHOULD BE CORRECTLY CONFIGURED!!!


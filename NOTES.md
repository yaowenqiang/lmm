> Linux Monitoring and Maintenance
> LPIC-1 117-101 117-102
> LPIC-2 117-2-1 117-202


# LPIC-2 201

+ Linux Monitoring and Maintenance(LPIC_2)
  + Capacity Planing
  + Advanced Network
  + System Maintenance
+ Linux Kernel and System Start Up(LPIC-2)
  + Linux Kernel
  + System Start Up
+ Linux Advance File System Management(LPIC-2)
  + File System and Devices
  + Advance Storage Administration



## Command Line Tools from sysstat

### vmstat

> vmstat -S M
> ls -R / # will increase memory buffered
> free -m
> sync
> sudo bash -c "echo 3 > /proc/sys/vm/drop_caches"
> free -m
> vmstat 5  3
> uptime
> who -l
> who -T

> root     + pts/0        2022-06-24 18:42 (61.144.189.155)  # + means message is turned on

> mesg n # turn mesg off
> tty
> mesg y # turn mesg on

> netstat -alt # list all listend tcp connection
> netstat -alx # list all listend socket
> ls -lh /var/run/dbus/system_bus_socket
> srwxrwxrwx 1 root root 0 Nov 13  2021 /var/run/dbus/system_bus_socket  # s means socket
> ps -elf
> netstat -alt # list connections on listening TCP
> sudo lsof -i 
> netstat -i 
> netstat -s
> sudo iptables -nvL
> watch -d sudo iptables -nvL # changes will be highlighted
> yum install sysstat
> cat /etc/cron.d/sysstat


> sar -V
> sar or sar -u
> sar -q
> sar -q 1 3
> sar -q -f /var/log/sa/sa15 (CentOS)
> sar -q -f /var/log/sysstat/sa15 (Ubuntu)
> sar -w
> sar -n DEV
> sar -q -s 10:00:00 -e 11:00:00



## using collectd to graph system performance

> yum install collectd collect-rrdtool rrdtool collectd-web httpd
> /etc/collectd.conf

## Monitoring availability with Nagios
## Basic networking and Wireless LAN
## Advanced network administration
## Project Building a Raspberry Pi Wireless Access Point
## Building from source
## Backup your data
## Ways to notify users


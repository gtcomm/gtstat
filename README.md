# gtstat
A new tool was created for everyone to use on any server to monitor web traffic and server resources at a glance.

## Description
It allows you to quickly view the following metrics of a server:

- Server uptime
- Server load
- Server kernel
- Global CPU Usage
- Global RAM Usage
- Global SWAP Usage
- Disk IOPS (read/write)
- Disk partitions over 80%
- Detected storage type (hard drive or flash based)
- Network port speed and bandwidth used (for wan port)
- Total number of requests to port 80 (and amount of ips generating them)
- Total number of requests to port 443 (and amount of ips generating them)
- Total number of established connections on port 80
- Total number of established connections on port 443
- List of the IP's generating the most requests

## Requirements
This script relies on a few components to be able to run. The software is made to run on RHEL or Debian based distributions.
It is also recommended to run this as root to ensure you can collect all the necessary data.
- sar
- netstat
- bc
- lsblk
- ethtool
- basic system utilities such as grep, free, fdisk, sort, cut, awk, uptime etc...

## Installation
The tool can be deployed with the following commands:
```
wget https://raw.githubusercontent.com/gtcomm/gtstat/master/gtstat -O /usr/bin/gtstat
chmod +x /usr/bin/gtstat
```
## Usage
Launch it with the following command:
```
gtstat
```

## Credits
This code was derived and improved from vdstat by duy13 (https://github.com/duy13/VDSTAT) for usage at GloboTech.

## GloboTech
GloboTech is a canadian hosting services provider based in Montreal. We offer bare metal and cloud based hosting solutions combined with best in class technical support to suit all your needs. Our team is dedicated since 1999 to provide an all inclusive environment for our business customers so they can strive without worrying about their technical challenges.

Visit our website at www.globo.tech today to get yourself a new server!

# Network Configuration and Troubleshooting Guide

## List Network Interfaces and IP Configuration

### Find the CLI Command to List the Network Interfaces

To list the network interfaces on a Windows system, use the `ipconfig` command.

### List All Network Interfaces on the System

```sh
ipconfig /all
```
### Manually Assign IP Addresses

To set a static IP address, use the following commands:

```sh
netsh interface ip set address "Ethernet0" static 192.168.1.10 255.255.255.0 192.168.1.1
netsh interface ip set dns "Ethernet0" static 8.8.8.8
netsh interface ip add dns "Ethernet0" 8.8.4.4 index=2
```
### Ping a Remote Server

To ping a remote server, use the following command:

```sh
ping -n 5 www.google.com
```
### Perform a Traceroute to a Remote Server

To perform a traceroute, use the following command:
```sh
tracert www.google.com
```


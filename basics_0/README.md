# Networking Basics

## Description

This project introduces the fundamental concepts of computer networking. It covers the OSI model, network types, IP and MAC addresses, TCP and UDP protocols, ports, and network connectivity testing using ICMP and ping.

The goal is to understand how devices communicate over networks and to gain basic experience with networking tools and Bash scripting.

## Requirements

* Ubuntu 22.04 LTS
* Bash scripts
* All files end with a new line
* All Bash scripts are executable
* All scripts start with:

```bash
#!/usr/bin/env bash
```

* The second line contains a comment describing the script
* Scripts pass ShellCheck without errors

## Files

| File                         | Description                                                |
| ---------------------------- | ---------------------------------------------------------- |
| 0-OSI_model                  | Answers related to the OSI model                           |
| 1-types_of_network           | Answers related to LAN, WAN, and Internet                  |
| 2-MAC_and_IP_address         | Answers related to MAC and IP addresses                    |
| 3-UDP_and_TCP                | Answers related to TCP and UDP                             |
| 4-TCP_and_UDP_ports          | Displays listening TCP/UDP ports with associated processes |
| 5-is_the_host_on_the_network | Pings a host 5 times using ICMP                            |

## Usage

### Make Scripts Executable

Before running the scripts, give them execution permissions:

```bash
chmod +x 4-TCP_and_UDP_ports
chmod +x 5-is_the_host_on_the_network
```

### Run File 4

Display all listening TCP and UDP ports, including the PID and program name associated with each socket:

```bash
sudo ./4-TCP_and_UDP_ports
```

Example output:

```text
tcp        0      0 *:ssh        *:*      LISTEN      1240/sshd
udp        0      0 *:bootpc     *:*                  562/dhclient
```

### Run File 5

Ping a host 5 times using ICMP:

```bash
./5-is_the_host_on_the_network 8.8.8.8
```

Example:

```text
PING 8.8.8.8 (8.8.8.8)
64 bytes from 8.8.8.8: icmp_seq=1 ttl=63 time=10 ms
...
```

If no IP address is provided:

```bash
./5-is_the_host_on_the_network
```

Output:

```text
Usage: 5-is_the_host_on_the_network {IP_ADDRESS}
```

## Networking Concepts Covered

### OSI Model

The OSI model is a conceptual framework used to understand network communications through seven layers.

### LAN

A Local Area Network connects devices within a limited geographic area such as a home, office, or school.

### WAN

A Wide Area Network connects multiple LANs across larger geographic areas.

### Internet

The global network that connects millions of devices worldwide.

### MAC Address

A unique hardware identifier assigned to a network interface.

### IP Address

A logical address used to identify devices on a network.

### TCP

A reliable transport protocol that guarantees packet delivery.

### UDP

A faster transport protocol that does not guarantee packet delivery.

### ICMP

A protocol used for diagnostics and connectivity testing, commonly through the ping command.


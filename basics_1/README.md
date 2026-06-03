# Networking Basics 1

This project focuses on basic networking concepts and Bash scripting in Ubuntu 22.04. It introduces tools and commands used to inspect and manipulate network behavior on a Linux system.

## Learning Objectives

At the end of this project, you should be able to explain:

- What is localhost / 127.0.0.1
- What is 0.0.0.0
- What is the /etc/hosts file
- How to display active network interfaces on a machine
- How to listen on a specific port using Netcat

## Requirements

- Allowed editors: vi, vim, emacs
- Scripts interpreted on Ubuntu 22.04
- All files must end with a new line
- A README.md file at the root of the project is mandatory
- All Bash script files must be executable
- Scripts must pass Shellcheck (version 0.7.0) without errors
- First line of all Bash scripts: `#!/usr/bin/env bash`
- Second line must be a comment describing the script

## Project Files

### 0. Change your home IP
File: `0-change_your_home_IP`  
Changes hostname resolution in `/etc/hosts` so that:
- localhost resolves to 127.0.0.2  
- facebook.com resolves to 8.8.8.8  

### 1. Show attached IPs
File: `1-show_attached_IPs`  
Displays all active IPv4 addresses on the machine, one per line.

### 2. Port listening on localhost
File: `2-port_listening_on_localhost`  
Listens on port 98 on localhost and prints any data received via a network connection.

---

## Repository Structure

| File | Description |
|------|-------------|
| `0-change_your_home_IP` | Modifies `/etc/hosts` to change localhost and facebook.com IP resolution |
| `1-show_attached_IPs` | Displays all active IPv4 addresses on the machine |
| `2-port_listening_on_localhost` | Listens on port 98 on localhost and prints received data |

---
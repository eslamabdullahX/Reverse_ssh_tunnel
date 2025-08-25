# RForward.py: A Python Reverse SSH Tunnel

A command-line tool written in Python to create a reverse SSH tunnel, allowing you to expose a local network service from behind a NAT or firewall. This script emulates the functionality of `ssh -R`.

This tool is perfect for penetration testing, remote administration, or giving temporary access to a local development server.



## Features

* **Exposes any local TCP port** to a remote server.
* **Multi-threaded architecture** to handle concurrent client connections gracefully.
* **Supports both password and public key** SSH authentication.
* **Configurable command-line interface** for easy setup of ports, hosts, and authentication methods.
* **Verbose mode** for debugging connection issues.

## Requirements

* Python 3.6+
* Paramiko library

## Installation

1.  Clone the repository (or simply download `rforward.py`).
    ```bash
    git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
    cd your-repo-name
    ```

2.  Install the required library:
    ```bash
    pip install paramiko
    ```

## Usage

The script is run from the command line with options to specify the ports and hosts.

**Syntax:**
```bash
python rforward.py [options] user@ssh-server[:port]

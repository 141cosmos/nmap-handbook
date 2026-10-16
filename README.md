# Nmap Beginner Handbook

A beginner-friendly handbook documenting my Nmap commands, networking concepts, and authorized scanning practice.

---

## 1. Check Nmap Version

**Command:**

```bash
nmap --version
```

**Purpose:** Checks whether Nmap is installed and displays its version information.

**What I learned:** The `--version` option displays information about the installed Nmap program.

---

## 2. Scan My Own Computer (Localhost)

**Command:**

```bash
nmap 127.0.0.1
```

**Purpose:** Scans my own computer's localhost address for common TCP ports.

**Key concepts:**

- `127.0.0.1` is the IPv4 loopback address.
- A port is a communication endpoint used by network services.
- An open port indicates that a service is listening for connections.
- Nmap's reported service name is an identification, not proof of a vulnerability.

**My scan results:**

- Date: 16 October 2026.
- Target: `127.0.0.1`
- Open ports:
  PORT   STATE SERVICE
135/tcp  open  msrpc
445/tcp  open  microsoft-ds
1042/tcp open  afrog
3306/tcp open  mysql
5357/tcp open  wsdapi
7778/tcp open  interwise
- What I learned: My first localhost scan showed that a computer can have multiple network ports in different states.

Key observations:

Ports allow applications and services to communicate over a network.

Nmap can identify open ports and report associated services.

An open port is not automatically a vulnerability.

Unexpected open ports may deserve further investigation.

Nmap can assist with network reconnaissance, but it is not a replacement for antivirus or dedicated malware analysis tools.

Security lesson: Always investigate suspicious services in context instead of assuming that every open port indicates malware.
---

*All scans in this handbook are performed against my own computer or systems I have explicit permission to test.*

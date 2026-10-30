# 🐧 Linux Server Administration Lab

A hands-on Linux system administration project designed to demonstrate practical skills in **Linux administration, troubleshooting, networking, security, service management, automation, and technical documentation**.

The project is built around a Debian Linux server and simulates tasks commonly performed by a:

- Junior Linux System Administrator
- Linux Support Engineer
- Linux Technical Support Engineer
- Application Support Engineer
- Junior Systems Engineer
- Cloud Support Engineer

This project is also designed to reinforce the knowledge required for **LPIC-1** through practical, real-world scenarios.

---

## 🎯 Project Objectives

The main objective of this project is to build and document a complete Linux administration laboratory from scratch.

Throughout the project, I will practice:

- Linux system administration
- Command-line usage
- File and directory management
- Users and groups
- File ownership and permissions
- ACLs
- Package management
- Process management
- System resources
- Networking
- DNS troubleshooting
- SSH administration
- Systemd and service management
- Log analysis
- Storage management
- Firewall configuration
- Linux security hardening
- Bash scripting
- System monitoring
- Incident troubleshooting
- Technical documentation

The project is intentionally designed as a **hands-on lab**, rather than simply a collection of theoretical exercises.

---

# 🏗️ Lab Architecture

The initial architecture consists of an administration machine connected to a Debian Linux server.

```text
                    ┌─────────────────────────┐
                    │      Admin Machine      │
                    │                         │
                    │  • Terminal             │
                    │  • Git                  │
                    │  • SSH Client           │
                    └────────────┬────────────┘
                                 │
                                 │ SSH
                                 │
                                 ▼
                    ┌─────────────────────────┐
                    │      Linux Server       │
                    │                         │
                    │      Debian GNU/Linux    │
                    │                         │
                    │  • Users & Groups       │
                    │  • Filesystem           │
                    │  • Networking           │
                    │  • OpenSSH              │
                    │  • systemd              │
                    │  • Firewall             │
                    │  • Logs                 │
                    │  • Services             │
                    └─────────────────────────┘

```
---

# 📂 Project Structure

```text

linux-server-administration-lab/
│
├── README.md
│
├── docs/
│   ├── installation.md
│   ├── users-and-groups.md
│   ├── permissions.md
│   ├── networking.md
│   ├── storage.md
│   ├── ssh.md
│   ├── services.md
│   ├── security.md
│   └── troubleshooting.md
│
├── scripts/
│   └── healthcheck.sh
│
├── configs/
│   └── linux-lab.service
│
└── screenshots/
    ├── system-info.png
    ├── users.png
    ├── networking.png
    ├── services.png
    └── firewall.png

```

# 🐧 Linux Administration

The server is configured and administered primarily through the Linux command line.

The project covers common administrative commands and utilities such as:

```

ls
cd
cp
mv
rm
find
grep
sed
awk
cat
less
tail
head
tar

```

System information and administration:

```

uname
hostnamectl
timedatectl
uptime
free
df
du
lsblk
findmnt

```

Process management:

```
ps
top
htop
kill
pkill

```




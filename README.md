Ubuntu Samba Network File Server

A simple, reliable way to turn Ubuntu 22.04 into a LAN-based file server that behaves like a Windows shared network folder, with full support for:

Linux, Windows, macOS clients

Auto-mounting on boot

Guest access or password-protected access

Multi-device file sharing

🚀 Features

✔ Easy Samba setup

✔ Windows-style shared folders

✔ Auto-mount on Linux clients

✔ Works across WiFi & LAN

✔ Supports guest access

✔ No software required on client side

| Topic                 | Link                                                   |
| --------------------- | ------------------------------------------------------ |
| Setup Samba Server    | [docs/SERVER_SETUP.md](docs/SERVER_SETUP.md)           |
| Connect Clients       | [docs/CLIENT_SETUP.md](docs/CLIENT_SETUP.md)           |
| Auto-Mounting on Boot | [docs/AUTO_MOUNT.md](docs/AUTO_MOUNT.md)               |
| Troubleshooting       | [docs/TROUBLESHOOTING.md](docs/TROUBLESHOOTING.md)     |
| Network Discovery     | [docs/NETWORK_DISCOVERY.md](docs/NETWORK_DISCOVERY.md) |



🛠 Technologies Used

Ubuntu 22.04

Samba (SMB server)

CIFS auto-mounting

gvfs (optional)


ubuntu-samba-file-server/
│
├── docs/
│   ├── SERVER_SETUP.md
│   │     ├─ Install Samba
│   │     ├─ Create share folder
│   │     └─ Configure smb.conf
│   │
│   ├── CLIENT_SETUP.md
│   │     ├─ Linux client
│   │     ├─ Windows client
│   │     └─ macOS client
│   │
│   ├── AUTO_MOUNT.md
│   │     ├─ fstab entry
│   │     ├─ test mount
│   │     └─ persistent mount
│   │
│   └── TROUBLESHOOTING.md
│         ├─ Network issues
│         ├─ Share name issues
│         └─ Mount errors
│
└── configs/
     └── smb.conf.example





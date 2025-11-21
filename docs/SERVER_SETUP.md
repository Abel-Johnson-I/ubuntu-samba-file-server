# Samba Server Setup (Ubuntu 22.04)

This guide explains how to configure your Ubuntu machine as a LAN file server.

---

## 1. Install Samba

```bash
sudo apt update
sudo apt install samba -y
```

---

## 2. Create the folder to share

```bash
mkdir -p /home/abel/shared_folder
chmod -R 777 /home/abel/shared_folder
```

---

## 3. Edit the Samba configuration

```bash
sudo nano /etc/samba/smb.conf
```

Add at the bottom:

```ini
[shared_folder]
   path = /home/abel/shared_folder
   browseable = yes
   read only = no
   guest ok = yes
   force user = abel
```

---

## 4. Restart Samba and verify

```bash
sudo systemctl restart smbd
sudo testparm -s
```

Expected output fragment:

```
[shared_folder]
    path = /home/abel/shared_folder
```

---

## 5. Check your IP

```bash
hostname -I
```

Use this IP for client connections.

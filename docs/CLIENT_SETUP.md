# Client Setup (Linux / Windows / macOS)

---

## Linux Clients

Open File Manager → Other Locations → Connect to Server:

```
smb://<SERVER-IP>/shared_folder
```

Test from terminal:

```bash
smbclient -L <SERVER-IP> -N
```

---

## Windows Clients

Open File Explorer → Address bar:

```
\\<SERVER_IP>\shared_folder
```

---

## macOS Clients

Finder → Go → Connect to Server:

```
smb://<SERVER_IP>/shared_folder
```

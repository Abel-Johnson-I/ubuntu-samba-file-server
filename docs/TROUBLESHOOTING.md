# Troubleshooting

---

## Error: NT_STATUS_HOST_UNREACHABLE

Cause:
- Wrong IP
- Server offline
- Different networks

Fix:
```bash
ping <SERVER-IP>
```

---

## Error: NT_STATUS_BAD_NETWORK_NAME

Cause:
- Incorrect share name
- Share not defined in smb.conf

Fix:
```bash
sudo testparm -s
```

---

## Error: mount point does not exist

Fix:
```bash
sudo mkdir -p /mnt/shared_folder
```

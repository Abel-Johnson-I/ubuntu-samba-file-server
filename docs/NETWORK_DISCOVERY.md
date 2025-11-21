# Network Discovery (Optional)

Make the Samba server appear under “Windows Network”.

---

## Install WSD service (Ubuntu)

```bash
sudo apt install wsdd
sudo systemctl enable --now wsdd
```

This makes the server visible on:

- Windows → Network  
- Linux → Networks  
- macOS → Network  

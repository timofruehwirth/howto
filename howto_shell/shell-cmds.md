## ClamAV

### Updating Signature Databases

```bash
freshclam
```

### One-Time Scanning

Scan all files in current directory
```bash
clamscan --recursive .
```

Scan all files on system
```bash
clamscan --recursive /
```
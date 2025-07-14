# 🛡 sigtrap — file integrity monitor written in C

Simple. Fast. Offline. No tracking. No telemetry. Just control.

## 🛠 Features

- Monitors file metadata:
  - `st_size` — file size
  - `st_mtime` — last modification time
  - `st_ctime` — metadata change time
  - `st_ino` — inode number
- Fully offline and private
- Lightweight static binary (Linux x86_64)
- No dependencies. No telemetry.
- Graceful exit message:
  > With silence and precision. — SilentPuck 🕶️

---

## 📥 Download

Get the latest release from the [Releases](https://github.com/SilentPuck/sigtrap/releases) section.

```bash
wget https://github.com/SilentPuck/sigtrap/releases/download/v1.0/sigtrap_v1.0.tar.gz
chmod +x sigtrap
```

> ✅ Recommended: use with read-only filesystems or immutable log setups.

---

## ⚙️ Usage

```bash
./sigtrap /path/to/file.log
```

After 5 seconds, `sigtrap` will detect:

- File size changes
- Metadata modifications
- Inode replacements

### 🧾 Example output:

```text
[*] Size changed: 1024 -> 2048
[*] Modified time changed
[!] Metadata changed
[!] Inode changed: 10765 -> 10902
```

---

## 💸 Support development

If this tool helps you — consider supporting future releases:

### 🟠 Monero (XMR)
```
46vt374N1tRduTQZFodskNbqygTnkFFo3SLJ8btmGkbyFpib65qFVMycF2PsDFpr1dUAv77JnpV5669HnRnULJ2Y6JkuFiS
```

### ₿ Bitcoin (BTC)
```
bc1q7jrq0u4yu6s5jgtrwkmwjaqhttam3ch3ura4aw
```
> 🕶 Privacy-first. No middlemen. No KYC.

---

## 🧠 Philosophy

**SilentPuck** builds silent tools for loud problems.  
No source. No tracking. No leaks. Just pure control.

> Invisible utilities for those who watch the watchers.

---

Made with 🛠 by [**SilentPuck**](https://github.com/SilentPuck)

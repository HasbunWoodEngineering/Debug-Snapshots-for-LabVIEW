# 🐞 Debug-Snapshots-for-LabVIEW
**Debug Snapshots for LabVIEW** is a lightweight Quick Drop tool that lets you save, restore, and clear the debug state of a VI — including breakpoints and probes — to quickly restore debugging contexts.

No dialogs, no UI clutter — just keyboard shortcuts.

---

## ✨ Features
- Save & restore breakpoints and probes
- Per-VI debug snapshots
- Optional breakpoint exclusion
- Simple cache management

---

## ⚡ Usage (Quick Drop)

### 💾 Save Debug Snapshot
- **Ctrl + S** — Save breakpoints & probes  
- **Ctrl + Shift + S** — Save *probes only* (ignore breakpoints)

### 🔁 Load Debug Snapshot
- **Ctrl + L** — Load snapshot  
- **Ctrl + Shift + L** — Load snapshot *without breakpoints*

### 🧹 Clear Debug Snapshot
- **Ctrl + C** — Clear snapshot for the active VI  
- **Ctrl + Shift + C** — Delete the entire snapshot cache file

---

## 🗂️ Cache File

The snapshot cache file path is stored in **LabVIEW.ini** under the key:


```DebugSnapshots.CacheFile```

By default, snapshots are stored in:

```C:\Users\<user>\Debug State Cache.xml```

You can overwrite this path manually if you want to use a different file.

---

## ⚠️ Limitations

- Restored probes are recreated through VI scripting and receive new probe numbers.

---

## 📦 Installation

### Users
If you only intend to use the tool, install it directly from  
**vipm.io**.

### Developers / Contributors
Clone the repository and open it with **JKI Dragon**.  
Dragon will automatically install all development dependencies defined in the [`Debug Snapshots for LabVIEW.dragon`](Debug%20Snapshots%20for%20LabVIEW.dragon) file.

---

## 📄 License
This project is released under the MIT License. See [LICENSE](LICENSE).

All relevant licenses (including development dependencies) are listed in [THIRD_PARTY_LICENSES](THIRD_PARTY_LICENSES).

---

## ⚠️ Disclaimer
LabVIEW™ is a trademark of National Instruments Corporation.

This project is an independent, open-source tool and is not affiliated with, endorsed by, or sponsored by National Instruments Corporation.
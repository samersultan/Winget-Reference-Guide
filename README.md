
### Show package details

```powershell
winget show <name>
```

---

## 📦 Install

### Install by name

```powershell
winget install <name>
```

### Install exact package (recommended)

```powershell
winget install --id <package.id> -e
```

### Silent install

```powershell
winget install --id <package.id> -e --silent
```

---

## ⬆️ Upgrade

### Check available updates

```powershell
winget upgrade
```

### Upgrade all packages

```powershell
winget upgrade --all
```

### Force + silent upgrade (recommended)

```powershell
winget upgrade --all --silent --force --accept-package-agreements --accept-source-agreements
```

### Upgrade specific package

```powershell
winget upgrade --id <package.id> -e
```

---

## ❌ Uninstall

### Uninstall by name

```powershell
winget uninstall <name>
```

### Uninstall exact package

```powershell
winget uninstall --id <package.id> -e
```

### Silent uninstall

```powershell
winget uninstall --id <package.id> -e --silent
```

---

## 📋 List Installed

```powershell
winget list
```

Filter:

```powershell
winget list <name>
```

---

## 📤 Export / Import

### Export installed apps

```powershell
winget export -o apps.json
```

### Import (install from list)

```powershell
winget import -i apps.json
```

---

## ⚙️ Useful Flags

| Flag                          | Description            |
| ----------------------------- | ---------------------- |
| `-e`                          | Exact match            |
| `--id`                        | Use package ID         |
| `--silent`                    | No UI                  |
| `--force`                     | Reinstall / override   |
| `--accept-package-agreements` | Auto accept terms      |
| `--accept-source-agreements`  | Auto accept sources    |
| `--include-unknown`           | Include untracked apps |

---

## 🧪 Troubleshooting

### Fix sources

```powershell
winget source reset --force
```

### If upgrade fails

```powershell
winget install --id <package.id> -e
```

---

## 🚀 Pro Tips

* Always use `--id` + `-e` for reliability
* Run upgrades regularly:

```powershell
winget upgrade --all
```

* Automate with Task Scheduler + `.ps1` script

---

## ⚡ One-Liner (Full Update)

```powershell
winget upgrade --all --silent --force --accept-package-agreements --accept-source-agreements --disable-interactivity
```

```
```

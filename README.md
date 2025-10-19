# PAPT (Modern APT Wrapper)

> A modern, colorful, and interactive wrapper around `apt`, designed to improve usability and provide a better user experience.
> Built by **Vyom Jain**.

---

## ✨ Features

-  **Colorful & Clean Output**
-  **Interactive Search & Install**
-  **finstall, fremove, fshow – Fast fuzzy actions**
-  **History & Snapshot System**
-  **Compare, verify, and GitHub install support**
-  **Progress bar with Pacman Animation**

---

## 📥 Installation

### 1. Clone / Download

```bash
git clone https://github.com/VyomJain6904/PAPT
cd PAPT
```

### 2. Move `papt` script to system path

```bash
sudo mv papt /usr/local/bin/papt
```

### 3. Make it executable

```bash
sudo chmod +x /usr/local/bin/papt
```

### ⚙️ (Optional) Set as Default APT Handler

**For Zsh (`~/.zshrc`)**
```bash
echo "alias apt='papt'" >> ~/.zshrc
source ~/.zshrc
```

**For Bash (`~/.bashrc`)**
```bash
echo "alias apt='papt'" >> ~/.bashrc
source ~/.bashrc
```

---

## PAPT Preview :

![PAPT Help](/assets/help.png)

### PAPT finstall :

![PAPT finstall](/assets/finstall.png)

### PAPT fremove :

![PAPT fremove](/assets/fremove.png)

### PAPT fshow :

![PAPT verify](/assets/verify.png)

### PAPT Compare :

![PAPT compare](/assets/compare.png)


## 🧠 Commands

| Command                 | Description                               |
| ----------------------- | ----------------------------------------- |
| `papt finstall`         | Interactive fuzzy install                 |
| `papt fremove`          | Interactive fuzzy remove                  |
| `papt fshow`            | Show package info interactively           |
| `papt history`          | View APT operations history               |
| `papt rollback`         | Rollback to previous snapshot             |
| `papt snapshots`        | List stored snapshots                     |
| `papt compare pkg1 pkg2`| Compare two packages                      |
| `papt verify <package>` | Verify package integrity                  |
| `papt github <url>`     | Install from GitHub repository            |

---

## 📦 Requirements

| Feature                        | Depends On                                |
| ------------------------------ | ----------------------------------------- |
| `finstall`, `fremove`, `fshow` | `fzf`, `batcat`   |
| Snapshot / Rollback            | Root access + `/var/log` write permission |
| GitHub Install                 | `git` + `make` (if building from source)  |

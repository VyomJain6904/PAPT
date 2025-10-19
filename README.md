## PAPT (Modern APT Wrapper)

`papt` is a modern wrapper around `apt` that enhances user experience with cleaner commands, colorful outputs, and improved usability.

### 1. Download / Copy the `papt` Script

### 2. Move it to `/usr/local/bin`

```bash
sudo mv papt /usr/local/bin/papt
```

3. Make it Executable

```bash
sudo chmod +x /usr/local/bin/papt
```

#### Optional – Replace apt with papt

To make papt your default APT handler, add this alias to your shell config.

For Zsh (.zshrc)

```bash
echo "alias apt='papt'" >> ~/.zshrc
source ~/.zshrc
```

For Bash (.bashrc)

```bash
echo "alias apt='papt'" >> ~/.bashrc
source ~/.bashrc
```

---

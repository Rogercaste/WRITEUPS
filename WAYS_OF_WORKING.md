# Ways of Working

## First Time Setup

```bash
# Configure git
git config --global user.name "Rogercaste"
git config --global user.email "your-email@example.com"

# Create local repo
mkdir ~/WRITEUPS
cd ~/WRITEUPS
git init
git branch -M main

# Add remote (token starts with ghp_)
git remote add origin https://Rogercaste:ghp_TOKEN@github.com/Rogercaste/WRITEUPS.git
```

## Generate a GitHub Token

1. GitHub → Profile pic → **Settings**
2. Scroll to **Developer settings**
3. **Personal access tokens** → **Tokens (classic)** → **Generate new token**
4. Check **repo** scope → Generate → Copy the `ghp_...` string

## Pushing a New Writeup

```bash
cd ~/WRITEUPS
cp /path/to/writeup.md .
git add .
git commit -m "Add <BoxName> writeup"
git push
```

## If Token Expires

```bash
git remote set-url origin https://Rogercaste:ghp_NEW_TOKEN@github.com/Rogercaste/WRITEUPS.git
```

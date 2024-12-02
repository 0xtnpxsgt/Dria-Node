# DRIA

# Prerequisites
- Operating System: Ensure you're running Linux (aarch64 or x86_64 architecture).
- Packages: Ensure curl and unzip are installed. If not, install them:

```bash
sudo apt update && sudo apt install -y curl unzip
```

1. Steps to Run the Script

```bash
wget https://raw.githubusercontent.com/0xtnpxsgt/Dria-Node/refs/heads/main/install-dkn-node.sh
```

2. Make the Script Executable: Give the script executable permissions:

```bash
chmod +x install-dkn-node.sh
```

3. Run the Script: Execute the script with:
```bash
./install-dkn-node.sh
```

- What the Script Does
Backups the .env File: If a .env file exists in the dkn-compute-node directory, it will back it up to .env.backup.

- Detects Your System Architecture:

- Downloads the appropriate binary (arm64 for ARM or amd64 for x86).
Downloads and Unzips the Node:

- Fetches the relevant ZIP file from GitHub.
Extracts it into the dkn-compute-node directory.
Restores the Backup .env File:

- Moves the .env.backup file back to .env.
Starts the Launcher:

Makes the launcher (dkn-compute-launcher) executable and runs it.

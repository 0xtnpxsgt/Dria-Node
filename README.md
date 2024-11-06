# Dria-Node  2.19


# One Click Install Explanation

1. Backup Existing .env: Checks if .env exists in the dkn-compute-node directory and creates a backup if it does.
2. Architecture Check: Uses uname -m to detect the system architecture (aarch64 or x86_64).
3. Download: Based on architecture, downloads the correct version of dkn-compute-launcher.
4. Extract & Navigate: Extracts the downloaded zip and navigates into the dkn-compute-node directory.
5. Restore .env Backup: If a backup exists, it’s restored to .env in the new node setup.
6. Run the Node: Gives the launcher execute permissions and starts it.


## Step 1:
```bash
sudo apt update
sudo apt install wget
wget https://raw.githubusercontent.com/0xtnpxsgt/Dria-Node/refs/heads/main/install-dkn-node.sh
```

## Step2:
```bash
chmod +x install-dkn-node.sh
./install-dkn-node.sh
```


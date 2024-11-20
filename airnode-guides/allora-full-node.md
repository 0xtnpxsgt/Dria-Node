---
icon: dice-three
---

# Allora Full Node

## Allora-Full-Node-Setup

![YF89\_m8Y-CXUWHpX](https://github.com/user-attachments/assets/f73c4212-73b2-473d-8be9-c64a13a588f0)

* You must need to buy a VPS for running Allora FULL NODE:
* You should buy VPS which is fulfilling all these requirements :

```bash
Operating System : Ubuntu 22.04
Recommended Hardware: 4 Cores, 8GB RAM, 200GB of storage (NVME)
```

#### Automatic Installation

```bash
cd $HOME
rm -rf install_allora.sh
wget https://raw.githubusercontent.com/0xtnpxsgt/Allora-Full-Node-Setup/main/install_allora.sh && chmod +x install_allora.sh && ./install_allora.sh
```

#### Check logs

```bash
docker compose logs -f
```

#### Check Sync Status

```bash
curl -s http://localhost:26657/status | jq .
```

#### Now you can use this RPC to your worker node:

```
To use this rpc for worker: http://YOURVPSIP:26657
```
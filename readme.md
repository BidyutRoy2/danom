# 🔥 DanomV4 Auto Installer

Automatic script to easily install and run **DanomV4 Testnet Worker**.

This script will:
- Install required dependencies
- Download and extract **DanomV4**
- Run **install.sh** from the server
- Prompt for **wallet address** and **Hugging Face API** input
- Save the configuration in `wallet_config.json`
- Start **Danom Worker** in a *screen session*

---

## 📥 **How ​​to Install**
### 1️⃣ Clone Repository
```bash
git clone https://github.com/BidyutRoy2/danom-node.git
cd danom-node
```

### 2️⃣ Grant Execution Permission
```bash
chmod +x install_danom.sh
```

### 3️⃣ Run Script
```bash
./install_danom.sh
```

### 4️⃣ Enter the Requested Data
When running the script, you will be asked to enter **wallet address** and **Hugging Face API**.

### 5️⃣ View Worker Processes
To enter a *screen* session and view running processes:
```bash
screen -Rd danom
```

If you want to exit *screen* without stopping the process:
```bash
CTRL + A + D
```

---

## 🏆 **Claim Reward and Swap**
- ✅ **Claim NOM No Fee:** [🔗 Testnet Claim](https://testnet.danom.site/)
- 💱 **Swap NOM to MON:** [🔗 Ambient Monad Swap](#) *(Link coming soon)*
- 📖 **Worker Documentation:** [🔗 Docs](https://testnet.danom.site/docs/how-it-work/howitwork)

---

## 🛠 **Troubleshooting**
- **If Danom is not running:**
```bash
screen -Rd danom
```
Make sure the process is still active in the screen.

- **If you want to restart the worker:**
```bash
pkill -f danom
screen -dmS danom ./danom
```

- **If there is an error during installation, try again with:**
```bash
rm -rf DanomV4.tar.gz Danom
./install_danom.sh
```

---

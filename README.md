# GENSYN-NODE-GUIDE (BY-NTEK-EARNING) 💖💖

## INSTALLATION COMMANDS (Only VPS) 👇🏻

---

# Gensyn Testnet Node Setup Guide

This guide walks you through setting up a Gensyn testnet node on a Ubuntu-based server.

---

## **Prerequisites**

Ensure your system is up to date:

```bash
sudo apt update
sudo apt install -y
```

Install required packages:

```bash
sudo apt update && sudo apt install -y python3 python3-venv python3-pip curl wget screen git lsof nano unzip iproute2
```

---

## **1. Install Node Dependencies**

```bash
curl -sSL https://raw.githubusercontent.com/zunxbt/installation/main/node.sh | bash
```

---

## **2. Start a Screen Session**

```bash
screen -S gensyn
```

---

## **3. Apply Fix Script**

```bash
curl https://raw.githubusercontent.com/imysryasir/Gsnyn-1-Click-Solutions/refs/heads/main/fixgensyn.sh | bash
```

---

## 4. Clone and Run Gensyn Node :

```bash
cd $HOME
rm -rf gensyn-testnet
git clone https://github.com/zunxbt/gensyn-testnet.git
chmod +x gensyn-testnet/gensyn.sh
./gensyn-testnet/gensyn.sh
```

---

## Main Error Solution (If Needed) :

```bash
curl https://raw.githubusercontent.com/imysryasir/Gsnyn-1-Click-Solutions/refs/heads/main/fixgensyn.sh | bash
```

---

## **5. Start RL Swarm :

```bash
cd rl-swarm
RL_SWARM_UNSLOTH=False ./run_rl_swarm.sh
```

---

## **6. Backup Your Node**

```bash
[ -f backup.sh ] && rm backup.sh
curl -sSL -O https://raw.githubusercontent.com/AbhiEBA/gensyn1/main/backup.sh
chmod +x backup.sh
./backup.sh
```

---

#### UPDATE NEW VERSION 😱😱

## **7. Node Management**

Here's a GitHub README guide for managing your **Gensyn** node using `screen`, particularly focusing on the `screen -r gensyn` command and related tasks:

---

# 🧠 Gensyn Node Setup & Management Guide

This guide helps you manage your Gensyn node using GNU Screen on a Linux VPS/server.

---

## 📦 Prerequisites

Ensure the following packages are installed:

```bash
sudo apt update && sudo apt install -y \
  python3 python3-venv python3-pip \
  curl wget screen git lsof nano unzip \
  iproute2 build-essential gcc g++
```

---

## 🚀 Start the Gensyn Node

```bash
screen -S gensyn
```

Then run your Gensyn node inside the screen:

```bash
# Clone and start Gensyn node
git clone https://github.com/zunxbt/rl-swarm.git
cd rl-swarm
./start.sh
```

(Adjust based on your actual start command if different.)

---

## 🔄 Inter Gensyn Screen :

```bash
screen -r gensyn
```

## Check screen sessions :

```bash
screen -ls
```

## Reattach to screen session :

```bash
screen -r
```

## Delete a screen session :

```bash
screen -S 65432.gensyn -X quit
```

### Remove existing swarm directory:

```bash
rm -rf rl-swarm
```

## 🔁 Step 1: System Preparation

### Install `sudo`

```bash
sudo apt update && sudo apt install -y sudo
```

### Install essential packages:

```bash
sudo apt update && sudo apt install -y \
  python3 python3-venv python3-pip curl wget screen git lsof \
  nano unzip iproute2 build-essential gcc g++
```

---

## ⚡ Step 2: Install CUDA

```bash
[ -f cuda.sh ] && rm cuda.sh
curl -o cuda.sh https://raw.githubusercontent.com/zunxbt/gensyn-testnet/main/cuda.sh
chmod +x cuda.sh
. ./cuda.sh
```

---

## 📦 Step 3: Install Node.js, Yarn, and Python Tools

```bash
sudo apt update && sudo apt install -y python3 python3-venv python3-pip curl wget screen git lsof

curl -fsSL https://deb.nodesource.com/setup_20.x | sudo -E bash -

sudo apt update && sudo apt install -y nodejs

curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -

echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list

sudo apt update && sudo apt install -y yarn
```

---

## ✅ Step 4: Verify Installations

```bash
node -v
npm -v
yarn -v
python3 --version
```

---

## 🖥 Step 5: Open a Screen Session

```bash
screen -S gensyn
```

---

## 📂 Step 6: Clone and Enter Swarm Directory

```bash
git clone https://github.com/gensyn-ai/rl-swarm.git && cd rl-swarm
```

---

## 🧪 Step 7: Set Up Python Virtual Environment

```bash
python3 -m venv .venv
source .venv/bin/activate
```

---

## 💻 Step 8: Set Up Frontend (modal-login)

```bash
cd modal-login

yarn install
yarn upgrade
yarn add next@latest
yarn add viem@latest

cd ..
```

---

## 📥 Step 9: Pull Latest Code & Checkout Specific Version

```bash
git reset --hard
git pull origin main
git checkout tags/v0.4.3
```

---

## 📝 Step 10: Edit Configuration File

```bash
nano hivemind_exp/configs/mac/grpo-qwen-2.5-0.5b-deepseek-r1.yaml
```

> After editing, press `CTRL + X`, then `CTRL + Y`, then `Enter` to save.

---

## 🚀 Step 11: Start RL-Swarm

```bash
RL_SWARM_UNSLOTH=False ./run_rl_swarm.sh
```

---

## 🌐 Step 12: Expose Frontend via LocalTunnel

### 1. Install LocalTunnel:

```bash
sudo npm install -g localtunnel
```

### 2. Start Tunnel on Port 3000:

```bash
lt --port 3000
```

### Useful Links**

* **Bot 1:** [Gensyn Track Bot](https://t.me/gensyntrackbot)
* **Bot 2:** [Gensyn Rewards Bot](https://t.me/gensyn_rewards_me_bot)
* **Explorer:** [Gensyn Explorer](https://gensyn-testnet.explorer.alchemy.com)
* **Dashboard:** [Gensyn Dashboard](https://dashboard.gensyn.ai/)
* **Telegram Channel:** [Join NTEK Earning](https://t.me/ntekearning


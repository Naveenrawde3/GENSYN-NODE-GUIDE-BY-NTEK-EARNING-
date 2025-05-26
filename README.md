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

## **4. Clone and Run Gensyn Node**

```bash
cd $HOME
rm -rf gensyn-testnet
git clone https://github.com/zunxbt/gensyn-testnet.git
chmod +x gensyn-testnet/gensyn.sh
./gensyn-testnet/gensyn.sh
```

---

## **Main Error Solution (If Needed)**

```bash
curl https://raw.githubusercontent.com/imysryasir/Gsnyn-1-Click-Solutions/refs/heads/main/fixgensyn.sh | bash
```

---

## **5. Start RL Swarm**

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

## **7. Node Management**

* **Check screen sessions:**

```bash
screen -ls
```

* **Reattach to screen session:**

```bash
screen -r
```

* **Delete a screen session (replace `65432.Gensyn` with your session name):**

```bash
screen -X -S 65432.Gensyn quit
```

---

## **8. Useful Links**

* **Bot 1:** [Gensyn Track Bot](https://t.me/gensyntrackbot)
* **Bot 2:** [Gensyn Rewards Bot](https://t.me/gensyn_rewards_me_bot)
* **Explorer:** [Gensyn Explorer](https://gensyn-testnet.explorer.alchemy.com)
* **Dashboard:** [Gensyn Dashboard](https://dashboard.gensyn.ai/)
* **Telegram Channel:** [Join NTEK Earning](https://t.me/ntekearning2)

---

Let me know if you'd like this saved to a file or styled further.


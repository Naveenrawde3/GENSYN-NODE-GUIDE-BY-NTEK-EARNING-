Here’s a clean and formatted version of your **Gensyn Node Guide** suitable for a GitHub README:

---

# GENSYN NODE GUIDE (BY NTEK EARNING)

A quick and simple guide to help you set up your Gensyn Node on a VPS.

---

## 🚀 Installation Commands (VPS Only)

```bash
sudo apt update
sudo apt install -y
sudo apt update && sudo apt install -y python3 python3-venv python3-pip curl wget screen git lsof nano unzip iproute2
curl -sSL https://raw.githubusercontent.com/zunxbt/installation/main/node.sh | bash
screen -S gensyn
curl https://raw.githubusercontent.com/imysryasir/Gsnyn-1-Click-Solutions/refs/heads/main/fixgensyn.sh | bash
cd $HOME && rm -rf gensyn-testnet && git clone https://github.com/zunxbt/gensyn-testnet.git
chmod +x gensyn-testnet/gensyn.sh
./gensyn-testnet/gensyn.sh
```

---

## 🧰 Troubleshooting

If you encounter any errors, try the following:

```bash
curl https://raw.githubusercontent.com/imysryasir/Gsnyn-1-Click-Solutions/refs/heads/main/fixgensyn.sh | bash
cd rl-swarm
RL_SWARM_UNSLOTH=False ./run_rl_swarm.sh
```

---

## 🔐 Backup Command

```bash
[ -f backup.sh ] && rm backup.sh
curl -sSL -O https://raw.githubusercontent.com/AbhiEBA/gensyn1/main/backup.sh
chmod +x backup.sh
./backup.sh
```

---

## 📟 Check Node Status (Next Day or Later)

```bash
screen -ls
screen -r
```

---

## ❌ Delete Screen

```bash
screen -X S 65432.Gensyn Quit
```

---

## 📊 Track Interactions

* **Bot 1:** [@gensyntrackbot](https://t.me/gensyntrackbot)
* **Bot 2:** [@gensyn\_rewards\_me\_bot](https://t.me/gensyn_rewards_me_bot)
* **Explorer:** [Gensyn Testnet Explorer](https://gensyn-testnet.explorer.alchemy.com)
* **Dashboard:** [Gensyn Dashboard](https://dashboard.gensyn.ai/)

---

## 📢 Join the Community

* [Telegram Channel](https://t.me/ntekearning2)

---

> Made with 💖 by NTEK Earning
> For educational and testnet purposes only.

---

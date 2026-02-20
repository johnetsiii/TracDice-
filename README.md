# 🎲 TracDice — P2P On-Chain Dice Casino

> A non-custodial, peer-to-peer dice gambling app built on [Intercom](https://github.com/Trac-Systems/intercom) — the Trac Network P2P agent sidechannel stack.

**Trac Address:** `trac1jqul5ff9w7mc5x0c4rc2gjuy09nd6y9pq47h9axunfu7k067yxksd6lgav`

---

## What is TracDice?

TracDice is a fully on-chain dice casino running over Intercom's P2P sidechannel infrastructure. Players bet **TNK tokens** against the house pool and roll dice in real-time. All randomness is verified on-chain via Trac Network's replicated-state layer.

### Game Modes
| Mode | Description | Payout |
|------|-------------|--------|
| **Exact Number** | Pick the exact dice face (1–6) | **5×** |
| **High / Low** | High = 4-6, Low = 1-3 | **2×** |
| **Even / Odd** | Even or Odd result | **2×** |

### Features
- 🔴 **Live P2P** — bets negotiated over Intercom sidechannels
- ⛓️ **On-chain settlement** — outcomes recorded in Trac replicated state
- ⚡ **Instant payouts** — TNK sent directly, no custodian
- 🎰 **Three bet modes** with different risk/reward
- 📊 **Live session stats** — W/L tracking, net P&L, streaks

---
<img width="1268" height="809" alt="image" src="https://github.com/user-attachments/assets/fc9801ff-bd29-415b-8671-23e9cc83abdf" />

## How It Works

```
Player → Intercom Sidechannel → House Agent → On-chain Commit → Reveal → Payout
```

1. Player submits bet + prediction via Intercom P2P message
2. House agent commits to a random seed on Trac replicated state
3. Dice result is revealed and verified
4. Winner receives TNK directly via Trac Network transfer

---

## Screenshots

> *(Add your screenshots here showing the app running)*

---

## Run Locally

```bash
git clone https://github.com/YOUR_USERNAME/intercom
cd intercom
# Open index.html in your browser for the UI demo
open index.html

# To run the full Intercom agent stack:
npm install
npm start
```

---

## Stack

- **Frontend:** Vanilla HTML/CSS/JS — `index.html`
- **P2P Layer:** [Intercom](https://github.com/Trac-Systems/intercom) sidechannels
- **Settlement:** Trac Network replicated state
- **Token:** TNK (Trac Network Token)

---

## Contributing

PRs welcome. See [awesome-intercom](https://github.com/Trac-Systems/awesome-intercom) for the full list of Intercom forks.

---

*Fork of [Trac-Systems/intercom](https://github.com/Trac-Systems/intercom)*

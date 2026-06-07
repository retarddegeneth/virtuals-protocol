# How to Run Vhermes

## 1. Prerequisites
- Terminal: bash
- Tools: git, gh (optional), node 18+ (if using ACP CLI), python 3
- Hermes Agent installed and configured

## 2. Configure the skillPATH
Option A: Use the Hermes skill system.
- hermes setup

Option B: Direct path.
- export HERMES_HOME="$HOME/.hermes"

## 3. Start the agent
- hermes run
- Select the `virtuals-protocol` skill / agent if prompted.

## 4. Example commands
- "Operator setup: create identity on Virtuals"
- "Fund the agent wallet"
- "Start an ACP deal"
- "Withdraw revenue to Base L1"

## 5. Verify
- hermes status
- hermes skills list

## 6. Troubleshoot
- WebError / no network: verify VPN or DNS.
- missing CLI: reinstall Hermes Agent.
- 401 on chain: confirm wallet is registered in EconomyOS.

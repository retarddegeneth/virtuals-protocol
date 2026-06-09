# Verifying command sources for Vhermes

If a Telegram bot command is referenced but not present in the repo, do not patch blindly. Run these checks in order:

1. Search the repo for command mentions with `gh search code "<term>" --repo OWNER/REPO --limit 50`
2. Check all raw files for command strings by fetching each tracked file
3. Check local bot handlers/skills for behavior hints
4. Ask for the exact definition URL or expected behavior before editing handlers

## /vtg status as of this session

- Confirmed absent from `retarddegeneth/virtuals-protocol` (searched tree + raw files + file search).
- Confirmed absent from local `~/vhermes-telegram-bot/handlers/onboarding.py`.
- Stored in this reference so future sessions do not repeat blind patches.

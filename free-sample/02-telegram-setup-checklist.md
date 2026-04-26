# Telegram Setup Checklist for OpenClaw

Use this checklist to get Telegram working cleanly without mixing direct-chat, group, and permission problems together.

---

## Phase 1. Bot creation

- [ ] Open `@BotFather`
- [ ] Create a new bot with `/newbot`
- [ ] Save the bot token safely
- [ ] Confirm you are configuring the correct bot

Important:
- the bot token is effectively a password;
- do not commit it to a public repo;
- revoke/regenerate it if leaked.

---

## Phase 2. OpenClaw config

- [ ] Add the Telegram bot token to config or environment
- [ ] Confirm `channels.telegram.enabled` is on
- [ ] Choose the DM access model: `pairing` or `allowlist`
- [ ] Do not use `open` unless you intentionally want a wide-open bot

Recommended first choices:

```text
First validation: pairing
Durable private bot: allowlist
Public/open bot: avoid unless intentional
```

---

## Phase 3. Direct-message validation

- [ ] Start the Gateway
- [ ] Send a message to the bot in direct chat
- [ ] If using pairing, approve the request
- [ ] If using allowlist, confirm your numeric Telegram user ID is in `allowFrom`
- [ ] Confirm the bot replies in DM before testing anything else

Do not start with groups.

---

## Phase 4. Owner authorization sanity check

- [ ] Confirm you know your numeric Telegram user ID
- [ ] Confirm you are not confusing username with user ID
- [ ] Confirm you are not confusing group ID with user ID
- [ ] If the bot is personal, prefer explicit numeric owner allowlist

Common mistake:

```text
@username != numeric Telegram user ID
```

---

## Phase 5. Group rollout

Only do this after DM works.

- [ ] Add the bot to one test group only
- [ ] Add the actual group chat ID under Telegram group config
- [ ] Keep `requireMention: true` for first tests
- [ ] Mention the bot explicitly when testing
- [ ] Do not put group IDs into user allowlist fields
- [ ] If restricting group usage, use numeric user IDs for allowed users

---

## Phase 6. Telegram-side settings

- [ ] If the bot must see all messages, review privacy mode in BotFather
- [ ] If privacy mode is changed, remove and re-add the bot to the group
- [ ] Only change privacy mode if always-on group visibility is really needed

For private assistants, mention-gated group behavior is usually safer.

---

## Fast failure map

If DM fails:

- [ ] check token
- [ ] check Gateway status
- [ ] check DM policy
- [ ] check pairing / allowlist
- [ ] check model path only after Telegram access is clearly working

If DM works but group fails:

- [ ] check group ID
- [ ] check mention gating
- [ ] check privacy mode
- [ ] check whether IDs are in the correct config fields

---

## Telegram success criteria

You are done when:

- [ ] bot replies in direct chat
- [ ] owner authorization is clear and explicit
- [ ] one test group works if needed
- [ ] group behavior is controlled, not noisy

---

## Full guide

The paid Launch Kit includes a complete Telegram setup guide with more examples, access model explanations, group behavior, and troubleshooting.

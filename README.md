# OpenClaw Personal Agent Starter Free

A free starter sample for technical users who want to build a private AI assistant in Telegram with OpenClaw.

The goal is simple:

> Get from “OpenClaw looks interesting” to a sane first private Telegram assistant path without guessing through every setup layer.

This repository is not a managed service and not a one-click installer. It is a practical preview of the paid **OpenClaw Telegram Assistant Launch Kit**.

---

## Start here

If you are new to this setup, read these in order:

1. [`free-sample/01-private-ai-assistant-starter-path.md`](free-sample/01-private-ai-assistant-starter-path.md)
2. [`free-sample/02-telegram-setup-checklist.md`](free-sample/02-telegram-setup-checklist.md)
3. [`free-sample/templates/AGENTS.md`](free-sample/templates/AGENTS.md)
4. [`free-sample/templates/SOUL.md`](free-sample/templates/SOUL.md)

Recommended first architecture:

```text
Personal PC
  + one strong model path
  + OpenClaw Gateway
  + Telegram direct messages
  + basic personal assistant persona
  + one real workflow tested
```

A boring working setup is better than an ambitious broken one.

---

## What you get in this free sample

```text
free-sample/
  01-private-ai-assistant-starter-path.md
  02-telegram-setup-checklist.md
  templates/
    AGENTS.md
    SOUL.md
paid-kit-preview/
  whats-inside.md
  free-vs-paid.md
```

The sample helps you understand:

- what a sane first OpenClaw assistant setup looks like;
- why Telegram direct chat is usually the best first channel;
- what can go wrong in Telegram setup;
- how workspace/persona files shape assistant behavior;
- whether the full paid kit is useful for you.

---

## What this helps you avoid

Common day-one mistakes:

- starting with Telegram groups before direct messages work;
- confusing Telegram usernames with numeric user IDs;
- changing model, deployment, persona, and channel config at the same time;
- trying weak local models before proving the workflow;
- treating `AGENTS.md` / `SOUL.md` as decorative prompts instead of operating rules;
- debugging the model when the real issue is Gateway, Telegram policy, or config.

---

## Who this is for

This sample is for:

- builders;
- self-hosting enthusiasts;
- indie hackers;
- developers;
- technical operators;
- AI power users;
- people who want a private assistant they can reach from Telegram.

It assumes you are comfortable editing config files and following technical setup steps.

---

## Who this is not for

This is probably not for you if:

- you want a fully managed SaaS;
- you do not want to touch config;
- you expect a one-click install;
- you want enterprise/team controls immediately;
- you expect weak local hardware to produce excellent model quality.

---

## Free guides

These pages explain the highest-friction parts of the setup:

- [OpenClaw Telegram setup guide](https://www.openclawlaunchkit.site/openclaw-telegram-setup-guide.html?utm_source=github&utm_medium=free_repo&utm_campaign=openclaw_starter_free)
- [Private AI assistant in Telegram](https://www.openclawlaunchkit.site/private-ai-assistant-telegram.html?utm_source=github&utm_medium=free_repo&utm_campaign=openclaw_starter_free)
- [OpenClaw model choice guide](https://www.openclawlaunchkit.site/openclaw-model-choice-guide.html?utm_source=github&utm_medium=free_repo&utm_campaign=openclaw_starter_free)

> Production landing domain is already set to `https://www.openclawlaunchkit.site`.

---

## Full Launch Kit

The paid kit is the complete self-serve setup package:

- Quick Start
- Personal PC deployment guide
- VPS deployment guide
- Local models guide
- Model choice guide
- Telegram setup guide
- Agent personality pack
- Troubleshooting guide
- Recommended starter builds
- Worked example: personal Telegram assistant
- Templates and persona overlays
- Launch, security, and Telegram checklists
- HTML release pack

Current MVP price target: **$29**.

Preview the full kit:

- [`paid-kit-preview/whats-inside.md`](paid-kit-preview/whats-inside.md)
- [`paid-kit-preview/free-vs-paid.md`](paid-kit-preview/free-vs-paid.md)

Landing page:

- [Get the full OpenClaw Telegram Assistant Launch Kit](https://www.openclawlaunchkit.site/?utm_source=github&utm_medium=free_repo&utm_campaign=openclaw_starter_free)

---

## Simple decision

Use this free sample if you are exploring.

Get the full kit if you already know you want a private OpenClaw assistant in Telegram and would rather follow a structured setup path than piece everything together from scattered docs.

---

## Important note

OpenClaw is active software. Always check the official OpenClaw documentation for breaking changes and current commands.

This sample gives you a practical starting model. It does not replace official docs.

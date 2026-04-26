# Private AI Assistant Starter Path

The fastest useful OpenClaw setup is usually not the most advanced one.

The goal of the first setup is simple:

> get to a private assistant you can message in Telegram, verify that it is useful, and only then add complexity.

---

## The recommended first path

Start with:

```text
Personal PC
  -> OpenClaw Gateway
  -> one strong model path
  -> Telegram direct chat
  -> basic personal assistant persona
  -> one real workflow
```

This gives you the shortest path to a setup that feels real.

---

## Why this path works

### 1. Personal PC first

A personal PC setup is easier to inspect and change while you are still learning the system.

A VPS can be useful later, but it adds extra variables:
- remote access;
- firewall/networking;
- service management;
- secrets handling;
- uptime/security concerns.

For a first working assistant, fewer variables is better.

### 2. One model path first

Do not start by comparing every model or building a complicated fallback chain.

Choose one good path:
- Codex-compatible auth if you already use it;
- direct API provider if you want predictability;
- OpenRouter if you want flexible model choice.

Local models are useful, but they can make the first experience worse if hardware/model quality is weak.

### 3. Telegram direct chat before groups

Direct chat validates the core loop:

```text
you send message -> OpenClaw receives it -> model replies -> Telegram returns response
```

Groups add more moving parts:
- group IDs;
- mention rules;
- bot privacy mode;
- per-group permissions;
- noisy context.

Prove direct messages first.

### 4. Simple persona before complex automation

A good assistant should have operating rules:
- how to answer;
- when to ask questions;
- how to handle ambiguity;
- what kind of outputs you prefer;
- what safety boundaries matter.

This is often more important than adding tools too early.

---

## A good first workflow

Pick one practical workflow and test it repeatedly.

Good examples:
- daily planning;
- task breakdown;
- technical troubleshooting;
- drafting small docs/configs;
- turning scattered notes into a checklist;
- summarizing a small research topic.

Bad first workflow:

> “automate everything in my life”

That is too broad to validate.

---

## First success criteria

Your first setup is successful when:

- OpenClaw Gateway runs;
- the model path works;
- Telegram direct chat replies;
- only the intended owner can use the bot;
- the assistant has a basic useful persona;
- one real workflow works more than once.

After that, you can decide whether to add:
- VPS deployment;
- Telegram groups;
- local models;
- more tools;
- recurring automation;
- richer memory/context.

---

## The rule

Do not optimize an assistant you have not made useful yet.

First make it work.
Then make it better.

# DWTS

**D**ump → **W**ork → **T**ransform → **S**tructure

A lightweight system to turn **scattered raw input** into **structured, styled output** — generating both **Markdown** and **HTML** (Bootstrap 5) with minimal user interaction.

---

## ⚠️ Critical: Commands vs Data

| Source     | Purpose                                            |
| ---------- | -------------------------------------------------- |
| `prompts/` | **SYSTEM COMMANDS** — instructions for AI behavior |
| `inbox/`   | **RAW DATA** — the actual content to process       |

---

## Automatic Flow

```
"DWTS" → Title? → Collection → Organize → Annotate? → Export
   ↑         ↑                                ↑
(trigger) (provide)                       (Yes/No)
```

**Only 2 user inputs needed:**

1. Document title
2. Yes/No for AI notes

Everything else runs automatically.

---

## How It Works

1. **Clone** this repo for each new project.
2. Dump raw material into `inbox/` — no formatting, no order.
3. Load `prompts/` files as context (these are commands, not data).
4. Send any message to start the process.
5. Provide title when asked.
6. Answer Yes/No for annotations.
7. Output is exported automatically as **both .md and .html**.

---

## What Gets Fixed

Each content type is represented with its **best UI representation**:

✅ Every component rendered optimally for readability  
✅ Proper formatting applied based on content type  
✅ Visual structure that matches the intent  
✅ Special characters and RTL text preserved

---

## What _Never_ Changes

❌ Your wording, voice, or intent  
❌ Links, images, embedded files  
❌ Meaning — even if phrased imperfectly

---

## Folder Structure

```
DWTS/
├── prompts/          # SYSTEM COMMANDS (not data!)
├── inbox/            # RAW DATA goes here
└── export/           # Output: .md + .html files
```

# DWTS

**D**ump → **W**ork → **T**ransform → **S**tructure

A multi-phase system to turn **scattered raw input** into **structured, styled output**.

---

## Folder Structure

```
DWTS/
├── prompts/          # Phase instructions (commands for AI)
├── inbox/            # RAW DATA goes here
└── export/           # Output: .md + .html files
```

---

## ⚠️ Critical: Commands vs Data

| Source     | Purpose                                           |
| ---------- | ------------------------------------------------- |
| `prompts/` | **PHASE COMMANDS** — instructions for AI behavior |
| `inbox/`   | **RAW DATA** — the actual content to process      |

---

## Phase System

Each phase is a **self-contained** instruction file in `prompts/`.

### Phase 01: Raw Extraction (`00_PHASE_01.txt`)

**What it does:**

-   Reads ALL files from `inbox/`
-   Represents each data type properly (lists, images, code, etc.)
-   Reorders blocks logically
-   Outputs to `export/` as `.md` and `.html`

**What it NEVER does:**

-   Fix typos, spelling, or grammar
-   Add words that weren't in source
-   Remove words that were in source

**Example:**

```
INPUT:  "too the zou go"
OUTPUT: "go too the zou"    ← Content preserved, just reordered
```

---

## How It Works

1. **Clone** this repo for each new project.
2. Dump raw material into `inbox/` — no formatting, no order.
3. Load the appropriate phase file from `prompts/` as context.
4. AI processes raw data according to phase instructions.
5. Output is exported to `export/` as **both .md and .html**.

---

## Phase 01 Details

| Action                        | Allowed |
| ----------------------------- | ------- |
| Read from `inbox/`            | ✅ YES  |
| Represent lists as lists      | ✅ YES  |
| Represent code as code blocks | ✅ YES  |
| Represent images as embeds    | ✅ YES  |
| Reorder blocks logically      | ✅ YES  |
| Fix typos                     | ❌ NO   |
| Fix grammar                   | ❌ NO   |
| Add explanations              | ❌ NO   |

# DWTS

**D**ump → **W**ork → **T**ransform → **S**tructure

A multi-phase system to turn **scattered raw input** into **structured, styled output**.

---

## 🚀 How to Use

### Step 1: Prepare Your Data

Put all your raw files into the `inbox/` folder. Can be any format, any structure.

### Step 2: Start New Session

Open a new AI chat session (Claude, Gemini, GPT, etc.)

### Step 3: Load Phase File

Copy the content of `prompts/00_PHASE_01.txt` and paste it as your first message, OR attach the file as context.

### Step 4: Trigger Execution

Send a message like:

```
Apply Phase 01 to the inbox folder.
```

or simply:

```
Execute Phase 01.
```

### Step 5: Get Output

The AI will process `inbox/` and create:

-   `export/output.md`
-   `export/output.html`

---

## Folder Structure

```
DWTs/
├── prompts/
│   └── 00_PHASE_01.txt    # Phase 1 instructions
├── inbox/                  # YOUR RAW DATA goes here
└── export/                 # Output files appear here
```

---

## ⚠️ Critical: Commands vs Data

| Source     | Purpose                                           |
| ---------- | ------------------------------------------------- |
| `prompts/` | **PHASE COMMANDS** — instructions for AI behavior |
| `inbox/`   | **RAW DATA** — the actual content to process      |

---

## Phase 01: Raw Extraction

**What it does:**

-   Reads ALL files from `inbox/`
-   Represents each data type properly (lists, images, code, etc.)
-   Reorders blocks logically
-   Outputs to `export/` as `.md` and `.html`

**What it STRICTLY NEVER does:**

-   ❌ Fix typos ("projct" stays "projct")
-   ❌ Fix spelling ("zou" stays "zou", NOT "zoo")
-   ❌ Fix grammar
-   ❌ Add words
-   ❌ Remove words
-   ❌ Add explanations or notes

**The Golden Rule:**

```
INPUT:  "too the zou go"
OUTPUT: "go too the zou"    ← Content preserved, just reordered
WRONG:  "go to the zoo"     ← VIOLATION (spelling was fixed)
```

---

## Quick Start Commands

After loading Phase 01 into a new session:

| Command            | What it does                    |
| ------------------ | ------------------------------- |
| `Execute Phase 01` | Process inbox and create output |
| `Apply Phase 01`   | Same as above                   |
| `Run Phase 01`     | Same as above                   |

---

## Tips for Stubborn AI Models

If a model keeps "fixing" things, try adding:

```
REMINDER: Do NOT fix ANY typos, spelling, or grammar.
The word "projct" must stay as "projct".
The word "zou" must stay as "zou".
I know there are mistakes. Keep them.
```

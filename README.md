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
Execute Phase 01.
```

### Step 5: Get Output

The AI will:

-   Create `export/phase_01.md` and `export/phase_01.html`
-   **CUT** (remove) the content from `inbox/` files

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

## Phase 01: What It Does (Quick List)

| #   | Action        | Details                                               |
| --- | ------------- | ----------------------------------------------------- |
| 1   | **Read**      | All files from `inbox/`                               |
| 2   | **Preserve**  | Content exactly as-is (Ctrl+F must find it)           |
| 3   | **Represent** | Lists as lists, code as code blocks, images as images |
| 4   | **Group**     | Related content into blocks/cards (smart grouping)    |
| 5   | **Title**     | Add simple headers (light purple highlight)           |
| 6   | **Style**     | Moderate theme (not dark, not light)                  |
| 7   | **Output**    | `phase_01.md` + `phase_01.html`                       |
| 8   | **CUT**       | Remove content from inbox files                       |

---

## Phase 02: Enhance & Structure

| #   | Action        | Details                                                 |
| --- | ------------- | ------------------------------------------------------- |
| 1   | **Read**      | Input from `export/phase_01.md`                         |
| 2   | **Correct**   | Fix typos ($ install), grammar, and formatting          |
| 3   | **Enhance**   | Convert raw text to Rich Components (Carousels, Tabs)   |
| 4   | **Structure** | Sidebar navigation + Anchors for every section          |
| 5   | **Diff View** | Interactive toggle: [Raw Phase 1] vs [Enhanced Phase 2] |
| 6   | **Output**    | `phase_02.md` (Clean) + `phase_02.html` (Interactive)   |

> **Critical Rule**: NO DATA LOSS. Phase 2 organizes and corrects, but it must NEVER delete user links, notes, or "scattered" thoughts. All data points must find a home in the new structure.

---

## Phase 01: What It NEVER Does

-   ❌ Fix typos ("projct" stays "projct")
-   ❌ Fix spelling ("zou" stays "zou")
-   ❌ Fix grammar
-   ❌ Add/remove words from raw content
-   ❌ Use complex vocabulary for titles

---

## Ctrl+F Test

**The #1 rule**: Copy any text from your raw files → Ctrl+F in output → Must find EXACT match.

If you can't find it, the AI violated the rules.

---

## Smart Grouping

Phase 01 groups content **smartly**:

✅ **RIGHT**: Keep questions with their related content

```
[Block: Flutter Setup]
- how to install flutter
- Q: what if it fails?
```

❌ **WRONG**: Group all questions together

```
[Block: Questions]
- Q: what if it fails? ← separated from context!
```

---

## Visual Highlights

-   **AI-added content** (titles, headers): Light purple background
-   **User raw data**: White/neutral background
-   **Theme**: Moderate (not dark, not very light)

---

## Tips for Stubborn AI Models

If a model keeps "fixing" things:

```
REMINDER: Do NOT fix ANY typos, spelling, or grammar.
The word "projct" must stay as "projct".
Ctrl+F from raw data must work in output.
```

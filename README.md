# DWTS

**D**ump → **W**ork → **T**ransform → **S**tructure

A multi-phase system to turn **scattered raw input** into **structured, styled output** using AI.

---

## 🎯 What This Does

You have messy notes, scattered thoughts, random links, code snippets, questions, and ideas all over the place. DWTS takes all of that chaos and transforms it into a beautiful, organized, searchable document.

### The Core Flow:

```
📥 INBOX (Raw Chaos) → 📦 PHASE 1 (Preserve & Group) → ✨ PHASE 2 (Enhance & Structure) → 📤 EXPORT
```

---

## 📁 Folder Structure

```
DWTs/
├── prompts/
│   ├── 00_PHASE_01.txt    # Phase 1 instructions (preservation)
│   └── 01_PHASE_02.txt    # Phase 2 instructions (enhancement)
├── inbox/                  # YOUR RAW DATA goes here
│   └── [your files]        # Any format: .txt, .md, images, etc.
├── export/                 # Output files appear here
│   ├── assets/             # Images and media
│   ├── phase_01.md         # Phase 1 Markdown output
│   ├── phase_01.html       # Phase 1 HTML output
│   ├── phase_02.md         # Phase 2 Markdown output (clean)
│   └── phase_02.html       # Phase 2 HTML output (interactive)
└── README.md               # This file
```

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

### Step 6: Run Phase 2 (Optional)

Start a new session, load `prompts/01_PHASE_02.txt`, and execute Phase 02.

---

## 📋 Phase Overview

### Phase 01: Raw Extraction (Preserve Everything)

| Action        | Details                                                 |
| ------------- | ------------------------------------------------------- |
| **Read**      | All files from `inbox/`                                 |
| **Preserve**  | Content exactly as-is (Ctrl+F must find it)             |
| **Represent** | Lists as lists, code as code blocks, images as images   |
| **Group**     | Related content into blocks/cards (smart grouping)      |
| **Title**     | Add simple headers (🟡 YELLOW highlight + 🤖 indicator) |
| **Style**     | Moderate theme (not dark, not light)                    |
| **Output**    | `phase_01.md` + `phase_01.html`                         |
| **CUT**       | Remove content from inbox files                         |

**Key Rule**: Phase 1 NEVER fixes typos, spelling, or grammar. "projct" stays "projct".

### Phase 02: Enhance & Structure

| Action            | Details                                                           |
| ----------------- | ----------------------------------------------------------------- |
| **Read**          | Input from `export/phase_01.md`                                   |
| **Correct**       | Fix typos, grammar, formatting (e.g., "$install" → "$ install")   |
| **Enhance**       | Convert to rich UI components (Tabs, Accordions, Timelines)       |
| **Track Changes** | Show what AI refined ✨, created 🤖, or omitted ~~strikethrough~~ |
| **Navigate**      | Sidebar with anchors + sub-anchors                                |
| **Raw Toggle**    | "Show Raw" button on every card                                   |
| **Output**        | `phase_02.md` (Clean) + `phase_02.html` (Interactive)             |

**Key Rule**: Phase 2 NEVER deletes data silently. All changes are tracked and visible.

---

## 🎨 Visual Conventions

### AI-Added Content Highlighting

| Type           | Visual Treatment                           | When Used                     |
| -------------- | ------------------------------------------ | ----------------------------- |
| 🤖 AI Created  | Yellow background (#fff3cd) + 🤖 indicator | Titles, headers, structure    |
| ✨ AI Refined  | Green background (#d4edda)                 | Typo fixes, grammar fixes     |
| ~~AI Omitted~~ | Gray strikethrough or collapsed section    | Removed duplicates, condensed |
| User Content   | White/neutral background (no highlight)    | Original raw data             |

### Phase 1 Example:

```html
<div class="ai-added">
	<span class="ai-indicator">🤖 AI</span>
	<h5>Flutter Setup</h5>
</div>
<div class="user-content">- how to install flutter - run flutter doctor</div>
```

### Phase 2 Example:

```html
<p>
	Use the <span class="ai-refined" title="was: instl">install</span> command.
</p>
<del class="ai-omitted">install install</del>
<!-- duplicate removed -->
```

---

## 🧩 UI Components (Phase 2)

Phase 2 uses the optimal UI representation for each type of content:

| Content Type        | Recommended Component        |
| ------------------- | ---------------------------- |
| Sequential steps    | Timeline / Ordered Steps     |
| Multiple options    | Tabs                         |
| FAQ / Questions     | Accordion                    |
| Commands            | Code block + Copy button     |
| Related links       | Badge list / Card grid       |
| Warnings/Notes      | Callout / Admonition         |
| Pros & Cons         | Two-column table             |
| Process flow        | Flowchart / Mermaid diagram  |
| Nested info         | Toggle / Collapsible section |
| Key terms           | Tooltip on hover             |
| Directory structure | File Tree                    |

### Full Block Types Available:

-   Text, Headings (1, 2, 3)
-   Card, Section, Highlight
-   Number list, Bullet list, Todo list
-   Toggle list, Toggle headings
-   Code block, Quote
-   Table, Image
-   Status Badge, Callout, Admonition
-   Tabs, Accordion, Tooltip
-   File Tree, Mermaid Diagram
-   KBD Shortcut, API Endpoint
-   Anchor Link, Table of Contents

---

## ✅ Ctrl+F Test (Phase 1)

**The #1 rule for Phase 1**: Copy any text from your raw files → Ctrl+F in output → Must find EXACT match.

If you can't find it, the AI violated the rules.

---

## 🔗 Smart Grouping (Phase 1)

Phase 1 groups content **smartly by context**, not by type:

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

## 🔀 Raw vs Enhanced (Phase 2)

Every card in Phase 2 has a toggle:

-   **Enhanced View** (default): Shows corrected, structured content with change indicators
-   **Raw View**: Shows the original Phase 1 content for comparison

This allows you to verify what the AI changed and approve the modifications.

---

## ⚠️ No Data Loss Policy

Across both phases:

-   Phase 1: Never fixes or removes anything
-   Phase 2: Never silently deletes — shows all changes visually
-   All links and URLs must be preserved
-   "Messy" data is polished, not hidden

---

## 🛠 Tips for Stubborn AI Models

If a model keeps "fixing" things in Phase 1:

```
REMINDER: Do NOT fix ANY typos, spelling, or grammar.
The word "projct" must stay as "projct".
Ctrl+F from raw data must work in output.
```

---

## 📊 Use Cases

This system works great for:

1. **Life Events / Memoir**: Random memories → Organized timeline
2. **Course Notes**: Scattered notes, questions, screenshots → Structured documentation
3. **Article Writing**: Collected ideas → Ready-to-publish draft
4. **CV/Resume**: Career fragments → Organized professional summary
5. **Project Planning**: Chaotic brainstorm → Clear project spec

---

## 🔄 Workflow Summary

```
┌─────────────────────────────────────────────────────────────────┐
│                        YOUR BRAIN DUMP                          │
│   (Notes, questions, links, code, images, random thoughts)      │
└─────────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────────┐
│                      📥 inbox/ folder                           │
│              Drop everything here (any format)                  │
└─────────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────────┐
│                     PHASE 1: PRESERVE                           │
│  • Group related content                                        │
│  • Add simple titles (🟡 yellow + 🤖)                           │
│  • Keep EVERYTHING exactly as-is                                │
│  • Output: phase_01.md + phase_01.html                          │
└─────────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────────┐
│                     PHASE 2: ENHANCE                            │
│  • Fix typos, grammar, formatting                               │
│  • Use optimal UI components                                    │
│  • Track changes: ✨ refined | 🤖 created | ~~omitted~~         │
│  • Add navigation with anchors                                  │
│  • Raw toggle on every card                                     │
│  • Output: phase_02.md + phase_02.html                          │
└─────────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────────┐
│                   📤 BEAUTIFUL OUTPUT                           │
│        Clean, structured, searchable documentation              │
└─────────────────────────────────────────────────────────────────┘
```

---

## 📝 License

MIT — Use it, modify it, share it.

---

## 🤝 Contributing

Feel free to improve the prompts or suggest better UI representations!

---

Made with 🧠 for turning chaos into clarity.

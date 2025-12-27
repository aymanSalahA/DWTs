# DWTS

**D**ump → **W**ork → **T**ransform → **S**tructure

A multi-phase system to turn **scattered raw input** into **structured, styled output** using AI.

---

## 🎯 What This Does

You have messy notes, scattered thoughts, random links, code snippets, questions, and ideas all over the place. DWTS takes all of that chaos and transforms it into a beautiful, organized, searchable document.

### The Core Flow:

```
📥 INBOX (Raw Chaos) → 📦 PHASE 1 (Preserve & Group) → ✨ PHASE 2 (Enhance & Structure) → 💡 PHASE 3 (AI Insights) → 📤 EXPORT
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
│   ├── assets/             # Project-specific asset folders
│   │   └── [timestamp_projectname]/  # e.g., 2024-01-15_flutter_notes/
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
| **Group**     | Related content into GRANULAR blocks/cards (10-20+)     |
| **Title**     | Add simple headers (🟡 YELLOW highlight + 🤖 indicator) |
| **Assets**    | Copy to `export/assets/[project]/`, reference only      |
| **Style**     | Moderate theme (not dark, not light)                    |
| **Output**    | `phase_01.md` + `phase_01.html`                         |
| **CUT**       | Remove content from inbox files                         |

**Key Rules for Phase 1**:

-   ❌ NEVER fixes typos, spelling, or grammar. "projct" stays "projct".
-   ✅ Creates MANY granular cards (10-20+), not few lumped blocks (3-5).
-   ✅ Assets are referenced but NOT analyzed/interpreted.

### Phase 02: Enhance & Structure

| Action            | Details                                                           |
| ----------------- | ----------------------------------------------------------------- |
| **Read**          | Input from `export/phase_01.md`                                   |
| **Correct**       | Fix typos, grammar, formatting (e.g., "$install" → "$ install")   |
| **Enhance**       | Convert to rich UI components (Tabs, Accordions, Timelines)       |
| **Track Changes** | Show what AI refined ✨, created 🤖, or omitted ~~strikethrough~~ |
| **Navigate**      | Sidebar with MANY categorized anchors + sub-anchors               |
| **Raw Toggle**    | "Show Raw" button on every card                                   |
| **Output**        | `phase_02.md` (Clean) + `phase_02.html` (Interactive)             |

**Key Rules for Phase 2**:

-   ❌ NEVER deletes data silently. All changes are tracked and visible.
-   ❌ NEVER adds AI hints, notes, or answers to questions (that's Phase 3!).
-   ✅ Sidebar has MANY categories (Resources, Workflow, Concepts, etc.).
-   ✅ Complex sections have sub-anchors (e.g., Process Steps → Step 0, Step 1, Step 2).

### Phase 03: AI Insights (Future)

This phase is where AI adds:

-   Answers to user's questions
-   Hints and suggestions
-   Links and recommendations
-   Clarifications and explanations

**Phase 2 edits the original data only. Phase 3 adds new AI-generated content.**

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

## 📊 Granular Grouping (Phase 1 — CRITICAL)

### The Golden Rule: MORE CARDS IS BETTER

Phase 1 must create MANY granular blocks, not few large ones.

| Input Size         | Expected Cards     |
| ------------------ | ------------------ |
| Small (1 page)     | 5-10 cards minimum |
| Medium (2-5 pages) | 10-20 cards        |
| Large (5+ pages)   | 20-50+ cards       |

❌ **WRONG (Gemini-style)**: 3-5 big blocks that lump everything together

```
[Card 1: Project Drafts] ← tons of content lumped here
[Card 2: Specifications]
[Card 3: Notes]
```

✅ **CORRECT (Opus-style)**: 10-20+ focused blocks

```
[Card 1: Tools Links]
[Card 2: Process Steps]
[Card 3: Questions]
[Card 4: Alternative Steps]
[Card 5: Project Notes]
[Card 6: Flutter Rules]
[Card 7: Main Idea]
[Card 8: Phases Info]
[Card 9: Requirements]
[Card 10: Open Questions]
[Card 11: Communication Style]
[Card 12: Images]
```

---

## 🧭 Navigation Sidebar (Phase 2 — CRITICAL)

### The Sidebar Must Be Detailed

The sidebar should look like a documentation website navigation, NOT just 3-4 links.

❌ **WRONG (too few categories)**:

```
- Drafts & Ideas
- Specifications
- References
```

✅ **CORRECT (detailed with categories and sub-anchors)**:

```
📁 Resources
   └─ Tools & Links

📁 Workflow
   └─ Process Steps
      ├─ Step 0: Submit
      ├─ Step 1: Order
      └─ Step 2: Group
   └─ Phase Details

📁 Concept
   └─ Mind Chaos Idea
   └─ Use Cases
   └─ Requirements

📁 Notes
   └─ Project Notes
   └─ Open Questions
   └─ Flutter Rules

📁 Media
   └─ Images
   └─ Attachments
```

---

## 📎 Assets & Attachments

### What Are Assets?

-   Images (PNG, JPG, WEBP, etc.)
-   PDFs
-   Excel files
-   Any attached files

### Asset Handling Rules

| Phase   | Rule                                                  |
| ------- | ----------------------------------------------------- |
| Phase 1 | Copy assets to `export/assets/[project]/`             |
| Phase 1 | Reference/embed assets (do NOT analyze their content) |
| Phase 2 | Display assets in appropriate cards                   |
| Phase 2 | Keep assets attached to their related cards           |

### Asset Folder Structure:

```
export/
└── assets/
    └── [timestamp]_[meaningful_name]/
        ├── screenshot.webp
        ├── diagram.png
        └── reference.pdf
```

Example: `export/assets/2024-01-15_flutter_notes/`

### What AI Should NOT Do With Assets:

-   ❌ Don't describe what's in an image
-   ❌ Don't summarize PDF contents
-   ❌ Don't interpret Excel data
-   ✅ Just reference/embed them as attachments

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

## 🚫 Phase 2 Does NOT Add AI Hints

This is a common mistake. Phase 2 is for EDITING, not for adding new AI content.

❌ **WRONG (adding AI hints/answers)**:

```html
<p>Q: What if flutter doctor fails?</p>
<p class="ai-created">🤖 AI Hint: Try reinstalling Flutter.</p>
```

✅ **CORRECT (just edit, no hints)**:

```html
<p>Q: What if Flutter Doctor fails?</p>
<!-- No AI answer - that's Phase 3 -->
```

If you want AI to answer questions or add suggestions, that's Phase 3.

---

## 🛠 Tips for Stubborn AI Models

### If the model creates too few cards in Phase 1:

```
REMINDER: Create MANY granular cards, not few big ones.
Target: 10-20+ cards, NOT 3-5.
Each topic/subject gets its OWN card.
```

### If the model keeps "fixing" things in Phase 1:

```
REMINDER: Do NOT fix ANY typos, spelling, or grammar.
The word "projct" must stay as "projct".
Ctrl+F from raw data must work in output.
```

### If the model creates too few sidebar categories in Phase 2:

```
REMINDER: Sidebar needs MANY categories with sub-anchors.
NOT: 3-5 links
CORRECT: 10+ links organized into sections (Resources, Workflow, Concepts, etc.)
```

### If the model adds hints/answers in Phase 2:

```
REMINDER: Phase 2 is for EDITING ONLY.
Do NOT add AI hints, notes, suggestions, or answers.
Questions stay as questions. That's Phase 3.
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
│  • Group into MANY granular cards (10-20+)                      │
│  • Add simple titles (🟡 yellow + 🤖)                           │
│  • Keep EVERYTHING exactly as-is                                │
│  • Assets: Copy & reference, don't analyze                      │
│  • Output: phase_01.md + phase_01.html                          │
└─────────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────────┐
│                     PHASE 2: ENHANCE                            │
│  • Fix typos, grammar, formatting                               │
│  • Use optimal UI components                                    │
│  • Track changes: ✨ refined | 🤖 created | ~~omitted~~         │
│  • Add MANY sidebar categories + sub-anchors                    │
│  • Raw toggle on every card                                     │
│  • ❌ NO AI hints/answers (that's Phase 3)                      │
│  • Output: phase_02.md + phase_02.html                          │
└─────────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────────┐
│                     PHASE 3: AI INSIGHTS (Future)               │
│  • Answer user's questions                                      │
│  • Add AI hints and suggestions                                 │
│  • Provide links and recommendations                            │
│  • Output: phase_03.md + phase_03.html                          │
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

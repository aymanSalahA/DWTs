# Phase 02: Enhanced Documentation

## 🛠 Tools and Resources

A curated list of markdown editors and tools mentioned in the raw data.

### Main Tools

-   **[Craft.do](https://www.craft.do/)** - Collaborative documents.
-   **[Easy Markdown Editor](https://github.com/Ionaru/easy-markdown-editor)** - Simple markdown editing.
-   **[Toast UI Editor](https://ui.toast.com/tui-editor)** - WYSIWYG Markdown editor.
-   **[Tiptap](https://github.com/ueberdosis/tiptap)** - Headless editor framework.
-   **[Saga.so](https://saga.so/use-cases/students)** - Knowledge management.

### Additional References (Recovered)

-   **[Markdown to PDF](https://www.markdowntopdf.com/)** - Tool for converting markdown files to PDF.
-   **[Qwen Chat Reference](https://chat.qwen.ai/c/536591b0-27ae-46cf-b078-503149711053)** - Context reference.

---

## 📈 Process Workflow

The defined "Metro Steps" for the project.

**Step 0: Submit Raw Data**

-   Input: Notes, bullet points, drafts, references.
-   User action required.

**Step 1: Order Data**

-   Suggest logical flow (Intro -> Body -> Conclusion).
-   **Rule:** No text edits allowed.

**Step 2: Group and Label**

-   Categorize related ideas.
-   **Rule:** Minor header/title edits allowed only.

**Step 3: Flag Gaps**

-   Identify redundancies or unclear sections.

**Step 4: Resolve Issues**

-   User must resolve flagged items.
-   **Rule:** No auto-fixing by AI without approval.

**Step 5: Final Approval**

-   Present ordered outline.

---

## 📝 Project Notes & FAQs

### Core Logic

**Flow:** `Collect` → `Organize` → `Fix` → `Export`

### Frequently Asked Questions

**Q: What if I add new raw info mid-process?**
A: You cannot proceed to the next step until the current one is finished. If new data is added, the process logic implies checking it against the current state (Collect phase).

**Q: What about the visual representation?**
A: Visuals are critical. The user prefers:

-   Flow charts / Graphs
-   Checklists / To-do lists
-   Embedded media (Images/Video)

**Q: What is the desired output format?**
A: A document structure (like a book) with chapters. It should be easy to view and search.

### AI Behavior Rules

-   **Sequential:** Do not skip phases.
-   **Brief:** Reply with single words like "Received" when in data collection mode.
-   **Titles:** Do not invent titles randomly.
-   **Formatting:** proper use of bold, italic, and multilingual support (Arabic).

---

## 💙 Flutter Documentation Rules

When organizing Flutter notes, apply these specific rules:

1.  **Preservation:** Keep original content exactly as written.
2.  **Categorization:** Use headings: "Page Layout", "Navigation", "Stateful vs Stateless", "Questions/TODOs".
3.  **AI Notes:** Highlight suggestions in yellow (e.g., `🟡 AI Note: [clarification]`).
4.  **Syntax Highlighting:** Ensure code blocks are properly tagged.
5.  **Output:** Single comprehensive Markdown file.

---

## 💡 Solution: Mind Chaos (Draft 1)

**Goal:** Create a solution for scattered ideas (Notion, Obsidian, Docs) that need to be collected, organized, and structured into a final document.

### Use Cases

1.  **Memoir:** Organizing random memories (1994, 2011, 1995) into a timeline.
2.  **Course Study:** Notes, questions, screenshots, and PDFs from a course.
3.  **Article Writing:** Collecting drafts and stories until ready to publish.
4.  **Career/CV:** Logging achievements over time.

### The 4 Phases

1.  **Phase 1 (Free Input):**

    -   Allow free writing.
    -   Data stays **RAW** (untouched).
    -   User feeds ideas continuously.

2.  **Phase 2 (Organize & Fix):**

    -   Group related info (e.g., linking a note from start to end of collection).
    -   AI suggests fixes (typos, spacing).
    -   **Crucial:** Raw data is preserved (strikethrough/highlight) until user accepts edits.

3.  **Phase 3 (Drafting):**

    -   (Implied from text) Structuring the content.

4.  **Final Phase (Export):**
    -   AI adds "Book-like" sections.
    -   AI adds explicit markers (e.g., 💡 Lamp icon) for its contributions.

### Requirements

-   **Output:** HTML or Markdown (user unsure, likely HTML for interactivity).
-   **Searchability:** Files must be easy to reference later.
-   **Communication:** Avoid "shitty talk". Be concise. List Pros & Cons.

---

## 🖼 Images

![User Asset](assets/kb-block-editor.webp)

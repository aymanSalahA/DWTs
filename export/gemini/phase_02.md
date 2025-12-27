# Phase 02: Enhancement & Organization

## Project Drafts

Now I want to create an idea for solving the "Mind Chaos Problem".

**Context:** Notion, Obsidian, and Google Docs exist for creating organized documents. However, for me, there is another issue: in some use cases, ideas, notes, or thoughts are scattered.
_Example:_ I write a note, then maybe some screenshots, then after a while write a question, then another note. Later, I understand and answer the first question.

### Use Cases

1.  **Life Events**: Imagine you remember your life: an event in 1994, then 2011, then 1995. You memorize them randomly but want to write an organized book with a timeline and titled chapters.
2.  **Course Notes**: Watching a course and keeping notes, writing questions to search later, adding PDFs, templates, screenshots, or cards.
3.  **Article Planning**: Planning to write an article by collecting ideas, stories, and everything related until it is ready.
4.  **Career/CV**: Writing a CV? You keep writing things about your career.

> **AI Note:** Since we talked about different cases, each case needs a different output file shape (or template), so putting this in consideration is important.

### Proposed Project Phases

First of all, as you can see, my thoughts even about this idea are scattered. Gathering my ideas and making a file with everything in my mind is a use case itself.

**Collect → Organize → Fix → Export**

-   **Phase 1: Free Input Mode**
    Allow free input where I can keep writing small (or big) notes. These notes/files should be **RAW** and untouched until this phase is done. I keep feeding ideas, and they are saved "Raw," exactly as-is.

-   **Phase 2: Organizing and Fixing**
    Organize and categorize notes (e.g., grouping related info from the beginning and end of Phase 1). Keep the content raw but grouped.
    _AI Role:_ Suggest fixes (redundant spaces, typos, repeated phrases). New edits should have marks (yellow highlight/strikethrough) while keeping raw data available until user approval.

-   **Final Phase: AI Sections**
    AI will add sections (like in books) with representation indicating AI content (e.g., a lamp icon). AI can put links for suggestions or answers below questions.

### Requirements & Questions

-   **Reference Quality**: Files should be good for future reference (easy to view/search).
-   **Visual Representation**: Use optimal representations (Todo lists, graphs, flowcharts, videos, image galleries, tables). Related to the "template" idea.
-   **Format**: HTML? Markdown? (Unsure).

**Q1: Is there an existing app for this?**
Is there something (app or whatever) that exists to do so?

**Q2: Best AI Model?**
What is the best AI model to do so? Or are all equal?

**Q3: Implementation Options?**
What is the best option? Coded project, Agent, Custom GPT, CLI? Or creating a bunch of prompts in a folder, running them with an AI editor to organize things?

---

## Specifications

-   **Step 0**: Submit raw data
-   **Step 1**: Order data (no text edits)
-   **Step 2**: Group and label (minor header edits only)
-   **Step 3**: Flag gaps, redundancies, unclear sections
-   **Step 4**: Resolve all flagged issues (user action required)
-   **Step 5**: Approve final outline

> **Rules:**
>
> -   No step proceeds until the current one is fully done and approved.
> -   Only Step 2 allows edits — and only to headers/titles. All body text stays 100% original.
> -   Step 4 flags must be resolved by you — no auto-fixing.
> -   Pause anytime. Resume later.

**Scenario Question:** What if after generating final data, the user adds a new piece of Raw info? Should we restart? What if the user wrote raw info in the middle of the process?

### Metro Steps & Requirements

User **CANNOT PROCEED** to the next metro step unless they finish the PREVIOUS step.
Example: Formatting for PDF, Visual hierarchy, Bilingual alignment.
[MarkdownToPDF](https://www.markdowntopdf.com/)

**User Workflow:**

1.  User gives scattered pieces of information.
2.  Organize them in the best order.
3.  Walk through until the final PDF file is obtained.
    **Important Note:** Keep raw data until the user asks to add or remove something.
    [Chat Qwen Link](https://chat.qwen.ai/c/536591b0-27ae-46cf-b078-503149711053)

---

## Notes & Prompts

**Phases:** Collect → Organize → Fix → Export. (If I give wrong order, it should be aware).

### Development Notes

1.  Phase 1 output shape: text in README (no checklists yet).
2.  Check representation options: Flow charts, etc.
3.  Phases must be sequential. No skipping unless under rules. AI reply: One word only (e.g., "Received"). No extra talk.
4.  Title must be known before starting (AI shouldn't make it up).
5.  Annotation/Markup needed (Bold, Italic, Second language support).
6.  Big files (Book-like) support? Or collect later?
7.  Support for images, media, and attachments.
8.  Code snippets: Need pretty image formatting (like HydePHP).
9.  Deduplication strategy: Remove later or keep?

### Prompt: Flutter Notes Organization

Organize my Flutter notes (text, code, images, todos) into a structured document. Follow these rules:

1.  Preserve my original content exactly as written.
2.  Categorize under headings: "Page Layout," "Navigation," "Stateful vs Stateless," "Questions/TODOs."
3.  Highlight AI notes/suggestions in yellow (e.g., "🟡 AI Note: [clarification]").
4.  For code, use syntax highlighting.
5.  Output: Generate both **Markdown**. Only one markdown that I can copy, including everything in one shot.

---

## References

-   [craft.do](https://www.craft.do/)
-   [Ionaru/easy-markdown-editor](https://github.com/Ionaru/easy-markdown-editor)
-   [ui.toast.com](https://ui.toast.com/)
-   [ui.toast.com/tui-editor](https://ui.toast.com/tui-editor)
-   [tiptap (GitHub)](https://github.com/ueberdosis/tiptap?spm=a2ty_o01.29997173.0.0.57a951712rRAIX)
-   [Saga.so Use Cases](https://saga.so/use-cases/students)

---

## Assets

![kb-block-editor](../inbox/dwt/kb-block-editor.webp)

# DWTs Project Documentation

## 💡 Core Idea: Solving Mind Chaos

I want to create an idea for solving the Mind Chaos Problem. Notion, Obsidian, and Google Docs exist if we want to create a document and we know what to write and how to organize. But for me there is another issue. In some use cases, the issue is that the ideas, notes, or thoughts are scattered.

**Example Scenario:** Write a note, then maybe some screenshots, maybe after a while write a question, maybe then write another note... maybe after the note I get another question and understand and get the answer for the first question I wrote... etc.

## 📋 Requirements

1. The files created should be good as a reference later if I need, easy to view and search inside.
2. The visual representation is very important, representing things I write into the correct and best representation. Maybe data are better as a todo list, checklist, graph, flowchart, embedded videos, image gallery, or tables. This is related to the "template" idea.
3. Since I talked about the representation, better to be HTML? Or Markdown? Or what? I don't know.

## 🔗 Competitors & Tools

-   [Craft.do](https://www.craft.do/)
-   [Saga.so (Use Cases)](https://saga.so/use-cases/students)
-   [Easy Markdown Editor](https://github.com/Ionaru/easy-markdown-editor)
-   [Toast UI Editor](https://ui.toast.com/tui-editor)
-   [Tiptap Editor](https://github.com/ueberdosis/tiptap)

## 💬 Communication Preferences

**Brief & Concise:** Please avoid long talk or making something seem like the "optimal solution". Provide pros and cons briefly.

I dislike talking so much and I want it as a conversation between me and a person. So when asking, make the response not too short nor too long.

## 🎯 Use Cases

1. **Life Events:** Imagine you remember your life: write an event at 1994, then event at 2011, then at 1995. You just memorize them randomly, but then you want to write an organized book about the events in a certain timeline and chapters with titles.
2. **Course Notes:** Watching a course and keep writing notes, writing questions of things to search later, putting some PDFs or templates or screenshots or cards for something, etc.
3. **Writing an Article:** Planning to write an article, and collecting ideas and stories and everything related, till it is ready to be an article.
4. **CV/Career:** Maybe also writing a CV? You keep writing things about the career?

## 📐 Output Shape & Templates

Since we talked about different cases, each case need a different output file shape (or in other words, a **template**), so also put this in consideration.

## 🚀 Submission Flow

-   **0 — Submit raw data**
-   **1 — Order data** (no text edits)
-   **2 — Group and label** (minor header edits only)
-   **3 — Flag gaps**, redundancies, unclear sections
-   **4 — Resolve all flagged issues** (user action required)
-   **5 — Approve final outline**

## ⚖️ Step Rules & Constraints

🔒 **No step proceeds** until the current one is fully done and approved.

-   ✍️ **Only Step 2 allows edits** — and only to headers/titles (e.g., shorten, clarify). All body text stays 100% original everywhere else.
-   🚩 **Step 4 flags must be resolved by you** — no auto-fixing by me. If something’s missing or unclear, I’ll stop and wait for your input.
-   ⏸️ **Pause anytime.** Resume later — your progress is saved at the last completed step.

## 📅 Project Phases (Draft)

-   **0 — User Raw Data:** Notes, bullet points, drafts, references, etc.
-   **1 — Order Data:** Suggest a logical flow (e.g., introduction → background → key points → conclusion), all letters/characters are untouched at all.
-   **2 — Categorize & Group:** Related ideas, add labels and titles and headers (minor edits in titles and category).
-   **3 — Flag Gaps:** Redundancies, or unclear sections for your review.
-   **4 — Present Outline:** The ordered outline (final draft) for approval.

**NOTE:** USER CAN'T PROCEED to next metro step unless they finish the PREV step.

## 🔄 Process Flowchart

[Collect] --> [Organize] --> [Fix] --> [Export]

If I give wrong order it should be aware.

## Phase 1: Collect / Free Input

**The Idea:** Allow free input mode, where I can keep writing small (or big) notes. Those notes or even files and documents should be **RAW**, not touched till this input Phase is Done.

So I keep feeding with my ideas and thoughts... etc. and they are saved "Raw", exactly as-is collecting first. Or Phase 1 can be a file with info but I will inject new ideas/notes/data inside it.

## Phase 2: Organizing and Fixing

This has lots of steps. For example, two pieces of info (one written at the beginning of the collect phase and one at the end) could be related and grouped under some title or category.

So this phase includes organizing and categorization of notes and data and grouping them. **But this Grouping still keeps them RAW and not touched.**

**AI Role:** Then comes the AI role, suggesting fixing (for example redundant spaces, or adding spaces, or fixing a typo, or even a phrase repeated twice and AI keeps only one). Although AI here is editing, the new edit should have some marks, and raw data should be kept (maybe with Strikethrough or highlight but kept) till user agree on the new edit.

## Phase 3: Final / Enhancement

AI will add sections (like the sections in books) where there is representation that this piece of paragraph or whatever is AI (maybe a lamp icon at the beginning).

Where AI can put links for suggestions or answers below questions or whatever.

## 📝 General Notes

1. The shape of the output is only text in README, no checklists even if it is better to represent it in the todo list shape.
2. Well, since we talk about shapes, what about flow charts and other representations too?
3. I want those Phases "Collect → Organize → Fix → Export." NOT escaped. It is sequential one by one, no skip unless under some rules ("fixing by AI for example"). Also for each phase AI reply with ONLY one word, so if in Collect, it always hint that it is in collected mode or if receive data it says "Received" (not bla bla at all).
4. Before anything, there is a need to know the title of the document, not AI making it up.
5. Annotation, or markup and making something bold or italic, or second language in doc like Arabic too.
6. Also if I want to make big file "that is like a book" will it be possible, or collect them later?
7. Images, media and attachments.
8. Code snippets, need them in pretty image like the ones in HydePHP.
9. Also need to remove duplicates later? Or keep it?

## ❓ Questions

**Q1: Is there something existing (app or whatever) to do so?**
A - question 1: is there something exist ( app or whatever ) to do so ?

**Q2: What is Best AI model to do so? Or all are equal?**
B - question 2 : What is Best AI model to do so ? or all are equal ?

**Q3: What is best option to cover those requirements?**
C - question 3 : what is best option to cover those requirements ? coded project , Agent or custom GPT , a CLI ?,Or creating a punch of prompts in a Folder and each time take those prompts in a new folder and open it with AI editor and put things ( files and write notes in files and put images and media ...etc )then make the Editor agent organize them ?

## ❓ Process Logic Q&A

**Ok, what if after generating final data, user added new piece of Raw info, should we restart? What if user wrote raw info in middle of process?**

## 🤖 Instructions to Agent

I will give you scattered pieces of Information, that need to be organized and then you give me the final Output.

1. Step one is that you get information and order them in best order.
2. After that I will walk you till we get final PDF file (I will tell you each step what is required in this phase).

**Important Note:** Keep my raw data till I ask you to add or remove something.

[Qwen Chat Link](https://chat.qwen.ai/c/536591b0-27ae-46cf-b078-503149711053)

## 📝 Flutter Notes Prompt

```
Organize my Flutter notes (text, code, images, todos) into a structured document. Follow these rules:
1. Preserve my original content exactly as written.
2. Categorize under headings: "Page Layout," "Navigation," "Stateful vs Stateless," "Questions/TODOs."
3. Highlight AI notes/suggestions in yellow (e.g., "🟡 AI Note: [clarification]").
4. For code, use syntax highlighting.
5. Output: Generate both **Markdown**. only one markown that I can copy , the markdown include everything in one shot
```

## 📎 Attachments

![kb-block-editor.webp](assets/2025-12-27_dwts/kb-block-editor.webp)

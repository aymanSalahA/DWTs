# DWTS Project - Phase 02 Enhanced Documentation

---

## 📋 Overview

### Main Concept - Mind Chaos Problem

I want to create an idea for solving the **Mind Chaos Problem**. While Notion, Obsidian, and Google Docs exist for creating documents when you know what to write and how to organize, there's another issue for me. In some use cases, the problem is that ideas, notes, or thoughts are scattered. For example: you write a note, then maybe some screenshots, maybe later a question, then another note, maybe after the note you get another question and understand and get the answer for the first question you wrote... etc.

---

## 🎯 Use Cases

### 1. Life Events Timeline

Let's imagine you remember your life: you write an event from 1994, then an event from 2011, then 1995. You memorize them randomly, but then you want to write an organized book about the events in a certain timeline with chapters and titles.

### 2. Course Notes Collection

Watching a course and keeping notes, writing questions of things to search later, putting some PDFs or templates or screenshots or cards for something... etc.

### 3. Article Planning

Planning to write an article and collecting ideas, stories, and everything related until it's ready to be an article.

### 4. CV Building

Maybe also writing a CV? You keep writing things about your career.

---

## 📐 Template Consideration

Since we talked about different cases, each case needs a different output file shape (or in other words, a template), so this should be put into consideration.

---

## 🔄 Project Phases

### Phase Overview

**Collect → Organize → Fix → Export**

### Phase 1: Collection

-   First of all, as you can see, my thoughts even about this idea are scattered. So gathering my ideas and making a file with all things in my mind about it is a use case.
-   The idea is to allow **free input mode**, where I can keep writing small (or big notes), and those notes or even files and documents should be **RAW**, not touched until this input phase is done. So I keep feeding with my ideas and thoughts, etc., and they are saved "Raw", exactly as-is. First, collecting. Or Phase 1 can be a file with info, but I will inject new ideas/notes/data inside it.

### Phase 2: Organizing and Fixing

Organizing and fixing has many steps. For example, two pieces of info - one written at the beginning of the collect phase and one written at the end - could be related and grouped under some title or category. This phase includes:

-   Organizing and categorization of notes and data
-   Grouping them (but this grouping still keeps them RAW and not touched)
-   AI role: suggesting fixes (e.g., redundant spaces, adding spaces, fixing typos, or removing repeated phrases)
-   Although AI is editing here, the new edit should have some marks, and raw data should be kept (maybe with strikethrough or highlight) until user agrees on the new edit.

### Final Phase: AI Enhancement

AI will add sections (like sections in books) where there is representation that this piece of paragraph is AI-generated (maybe a lamp icon at the beginning). AI can put links for suggestions or answers below questions.

---

## 🎯 Goals for Output Files

1. **Searchable Reference**: The files created should be good as a reference later, easy to view and search inside.
2. **Visual Representation**: Representing things I write into the correct and best representation. Maybe data is better as:
    - Todo list or checklist
    - Graph or flowchart
    - Embedded videos
    - Image gallery
    - Tables
    - This is related to the "template" idea.

---

## ❓ Format Question

Better to be HTML or Markdown or what? I don't know.

---

## 🔍 Open Questions

| #   | Question                                                                                                                                                                                                                                                                                                                                        |
| --- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| A   | Is there something that exists (app or whatever) to do so?                                                                                                                                                                                                                                                                                      |
| B   | What is the best AI model to do so? Or are all equal?                                                                                                                                                                                                                                                                                           |
| C   | What is the best option to cover those requirements? Coded project, Agent or custom GPT, a CLI? Or creating a bunch of prompts in a folder and each time take those prompts in a new folder and open it with AI editor and put things (files and write notes in files and put images and media, etc.) then make the editor agent organize them? |

---

## 💬 Communication Preference

Please avoid excessive talking or presenting something as the optimal solution. If you say something, be brief and concise and put pros and cons. I hate talking too much and I want it as a conversation between me and a person, so when asking, make the response not too short nor too long.

---

## 🔗 Competing Tools

| Tool                 | Link                                           |
| -------------------- | ---------------------------------------------- |
| Craft                | https://www.craft.do/                          |
| Easy Markdown Editor | https://github.com/Ionaru/easy-markdown-editor |
| Toast UI             | https://ui.toast.com/                          |
| Toast UI Editor      | https://ui.toast.com/tui-editor                |
| Tiptap               | https://github.com/ueberdosis/tiptap           |
| Saga                 | https://saga.so/use-cases/students             |

---

## 📈 Workflow Steps

### Version 1: Detailed Steps

| Step | Action                                            | Text Edits Allowed      |
| ---- | ------------------------------------------------- | ----------------------- |
| 0    | Submit raw data                                   | No                      |
| 1    | Order data                                        | No                      |
| 2    | Group and label                                   | Minor header edits only |
| 3    | Flag gaps, redundancies, unclear sections         | No                      |
| 4    | Resolve all flagged issues (user action required) | No                      |
| 5    | Approve final outline                             | No                      |

### Version 2: Alternative Steps

| Step | Action                                                                                                                      |
| ---- | --------------------------------------------------------------------------------------------------------------------------- |
| 0    | User raw data (notes, bullet points, drafts, references, etc.)                                                              |
| 1    | Order data / Suggest a logical flow (introduction → background → key points → conclusion), all letters/characters untouched |
| 2    | Categorize and group related ideas / Add labels, titles, and headers (minor edits in titles and category)                   |
| 3    | Flag gaps, redundancies, or unclear sections for review                                                                     |
| 4    | Present the ordered outline (final draft) for approval                                                                      |

---

## 🔒 Workflow Rules

-   🔒 No step proceeds until the current one is fully done and approved.
-   ✍️ Only Step 2 allows edits — and only to headers/titles. All body text stays 100% original everywhere else.
-   🚩 Step 4 flags must be resolved by you — no auto-fixing. If something's missing or unclear, I'll stop and wait for your input.
-   ⏸️ Pause anytime. Resume later — your progress is saved at the last completed step.

### Step Enforcement

**USER CANNOT PROCEED to next metro step unless finish the PREVIOUS step.**

---

## ❓ Question About New Data

What if after generating final data, user added a new piece of raw info? Should we restart? What if user wrote raw info in the middle of the process?

---

## 📤 Export Considerations

-   Formatting for PDF
-   Visual hierarchy
-   Bilingual alignment
-   Tool: https://www.markdowntopdf.com/

---

## 📝 Prompt Template

I will give you scattered pieces of information that need to be organized, and then you give me the final output.

Step one is that you get information and order them in the best order.

After that, I will walk you through until we get the final PDF file (I will tell you each step what is required in this phase).

**Important note:** Keep my raw data until I ask you to add or remove something.

---

## 🔗 Reference Chat

https://chat.qwen.ai/c/536591b0-27ae-46cf-b078-503149711053

---

## 📓 Notes After Testing

After making the agents and still having to try other models, here are the notes:

| #   | Note                                                                                                                                                                                                                                                                                                                 |
| --- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | The shape of the output is only text in readme, no checklists even if it's better to represent it in todo list shape                                                                                                                                                                                                 |
| 2   | What about flow charts and other representations too?                                                                                                                                                                                                                                                                |
| 3   | The phases "Collect → Organize → Fix → Export" should not be escapable. It's sequential, one by one, no skip unless under some rules. Also, for each phase, AI replies with ONLY one word. If in Collect, it always hints that it's in collected mode. If it receives data, it says "Received", not a long response. |
| 4   | Before anything, there's a need to know the title of the document, not AI making it up                                                                                                                                                                                                                               |
| 5   | Annotation or markup: making something bold or italic, or second language in doc like Arabic too                                                                                                                                                                                                                     |
| 6   | If I want to make a big file "that is like a book", will it be possible, or collect them later?                                                                                                                                                                                                                      |
| 7   | Images, media, and attachments                                                                                                                                                                                                                                                                                       |
| 8   | Code snippets need to be in pretty images like the ones in HydePHP                                                                                                                                                                                                                                                   |
| 9   | Need to remove duplicates later? Or keep them?                                                                                                                                                                                                                                                                       |

---

## 🎨 Flutter Notes Prompt Template

Organize my Flutter notes (text, code, images, todos) into a structured document. Follow these rules:

1. Preserve my original content exactly as written.
2. Categorize under headings: "Page Layout," "Navigation," "Stateful vs Stateless," "Questions/TODOs."
3. Highlight AI notes/suggestions in yellow (e.g., "🟡 AI Note: [clarification]").
4. For code, use syntax highlighting.
5. Output: Generate Markdown. Only one markdown that I can copy, the markdown includes everything in one shot.

---

## 📎 Attachments

![Block Editor Reference](assets/2024-12-27_dwts/kb-block-editor.webp)

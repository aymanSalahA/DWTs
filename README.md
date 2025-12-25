# DWTS  
**D**ump → **W**ork → **T**ransform → **S**tructure  

A lightweight system to turn **scattered raw input** (notes, questions, screenshots, files) into **structured, referenceable output** — without forcing early organization.

---

## Purpose

Collect chaos first. Structure later.  
AI assists *only after* raw capture is complete — never during.

---

## How It Works

1. **Clone** this repo for each new project (e.g. `git clone DWTS flutter-notes`).  
2. Dump raw material into `inbox/` — no formatting, no order.  
3. Run prompts in sequence:  
   - `collect` → inventory raw items  
   - `organize` → group & suggest structure (raw preserved)  
   - `fix` → propose edits (typos, commands, lists — changes marked)  
   - `export-{template}` → generate final doc (CV, article, book, etc.)  
4. Output lands in `export/`.

> 🔁 **Recursive**: Feed an `export/` file into a *new* `inbox/` to refine it further.

---

## What Gets Fixed (in `fix` phase)

✅ Commands → proper code blocks & spacing (`$ npm`, not `$npm`)  
✅ TODOs → `- [ ] TODO: ...`  
✅ Questions → prefixed with `**Q:**`  
✅ Typos → obvious fixes only (`projct` → `project`)  
✅ Lists → markdown syntax  
✅ Code → language-tagged blocks  
✅ Special chars → preserved (`╰─$`, RTL, etc.)

---

## What *Never* Changes

❌ Your wording, voice, or intent  
❌ Links, images, embedded files  
❌ Meaning — even if phrased imperfectly

---

## Folder Structure

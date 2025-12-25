## What is DWTS?

A lightweight system to turn **scattered raw input** (notes, questions, screenshots, files) into **structured, referenceable output** — without forcing early organization.

## Purpose

Help you collect chaos first, structure later — with AI assistance *only after* raw capture is complete.

---

## How it works

1. **Clone** this repo for each new document
2. Dump *anything* into `inbox/` — no formatting, no order.  
3. Run prompts in sequence:  
   - `collect` → inventory raw items  
   - `organize` → group & suggest structure (raw untouched)  
   - `fix` → propose edits (changes marked, original kept)  
   - `export-{template}` → generate final doc (CV, article, etc.)  
4. Results go to `export/`.

> 🔁 **Recursive**: You can feed an `export/` file back into a *new* `inbox/` to refine it further.
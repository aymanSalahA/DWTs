# Export Output Example

## What You Should Get When You Type "Export"

When you type "Export", the AI's ENTIRE response should look EXACTLY like this:

---

## ✅ CORRECT OUTPUT (Copy Everything Below):

````markdown
# Laravel-Livewire Chat-Message-App-Scratch (Course Notes)

## Chapter 1: Introduction

### Project Setup

First thing: creating new project

```bash
$ composer create-project laravel/laravel live-wire-chat
```
````

**Q:** Why `--dev`?

💡 `--dev` installs Breeze as a development dependency.

-   [ ] TODO: Check Volt and Livewire options

[... rest of your content ...]

```

---

## ❌ WRONG OUTPUT (What You DON'T Want):

```

Here's your organized document:

```markdown
# Laravel-Livewire Chat-Message-App-Scratch (Course Notes)

## Chapter 1: Introduction

[... content ...]
```

Let me know if you need any changes!

```

**Problem:** Extra text before and after the code block makes it impossible to copy cleanly.

---

## ⚠️ The Rule

**When you type "Export", the AI should respond with:**
1. ✅ ONLY the markdown code block
2. ✅ Nothing before it
3. ✅ Nothing after it
4. ✅ You can copy the ENTIRE response and paste it directly into a .md file

**The AI should NOT:**
1. ❌ Add "Here's your document"
2. ❌ Add "Let me know if you need changes"
3. ❌ Add ANY explanatory text
4. ❌ Break the content into multiple code blocks

---

## How to Use the Output

1. Type "Export"
2. AI responds with ONE code block
3. Click "Copy" button on the code block (or select all and copy)
4. Paste into your .md file
5. Done! ✅

---

## Testing

If the AI adds ANY text before or after the code block, the prompts need to be reinforced.

The ENTIRE response should be copyable as one complete markdown file.
```

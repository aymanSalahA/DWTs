# V2 Agent Quick Reference

## How to Use

### 1. Start a New Session

The agent will greet you and ask: **"Title?"**

Example response: `Laravel-Livewire Chat App Notes`

### 2. Feed Data Piece by Piece

Paste your raw notes, commands, thoughts, etc.

The agent will respond: **"Received"** (and nothing else)

### 3. Organize When Ready

Type: **"Organize"**

The agent will ask: **"Organizing... Annotate? (Yes/No)"**

### 4. Choose Annotation

-   Type **"Yes"** if you want AI to add helpful 💡 notes
-   Type **"No"** if you want just your content formatted

### 5. Export

Type: **"Export"**

You'll get a properly formatted markdown document ready to copy/paste.

### 6. Continue (Optional)

Type: **"More"** to add more content to the same document.

---

## What Gets Fixed Automatically

✅ **Commands**: Wrapped in code blocks with proper spacing
✅ **TODOs**: Converted to markdown checkboxes `- [ ] TODO:`
✅ **Questions**: Formatted with **Q:** prefix
✅ **Typos**: Obvious mistakes corrected (projct → project)
✅ **Lists**: Proper markdown list syntax
✅ **Code**: Proper code blocks with language tags
✅ **Spacing**: Command spacing fixed (`$ npm` not `$npm`)

---

## What Stays Exactly the Same

❌ Your wording and sentences
❌ Your meaning and intent
❌ Special characters (╰─$, etc.)
❌ Links, images, RTL text
❌ Your voice and style

---

## Example Session

```
Agent: Title?
You: Flutter Notes

Agent: Ready
You: [paste raw notes]

Agent: Received
You: [paste more notes]

Agent: Received
You: Organize

Agent: Organizing... Annotate? (Yes/No)
You: Yes

Agent: Annotating... Ready to Export.
You: Export

Agent: [outputs formatted markdown in code block]
```

---

## Commands Summary

| Command    | Purpose                                    |
| ---------- | ------------------------------------------ |
| `Title?`   | Start new document (agent asks this first) |
| `Organize` | Structure and format your fragments        |
| `Yes`      | Enable AI annotations (💡 notes)           |
| `No`       | Skip AI annotations                        |
| `Export`   | Get final formatted markdown               |
| `More`     | Continue adding to same document           |

---

## Tips

1. **Don't worry about formatting** while collecting - just paste raw content
2. **Feed incrementally** - paste one section at a time as you take notes
3. **Use "More"** to build up large documents over multiple sessions
4. **Copy the export** directly from the code block - it's ready to use
5. **Questions and TODOs** will be automatically formatted for clarity

---

## Formatting Examples

### Commands

Input: `$npm install`
Output:

```bash
$ npm install
```

### TODOs

Input: `TODO : check this later`
Output: `- [ ] TODO: Check this later`

### Questions

Input: `question : why use this?`
Output: `**Q:** Why use this?`

### Code Blocks

Input:

```
# comment
command here
```

Output:

```bash
# comment
command here
```

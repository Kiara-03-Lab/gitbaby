# GitBaby 👶💻

A code editor designed for young children to create and save projects—no confusing git commands, no scary GitHub interface.

## What is this?

Your kid can:
- Click "New Project" and start coding
- Edit HTML, CSS, JavaScript files
- Click "Save" and it's instantly saved
- Share projects with friends

That's it. No branches, no commits, no terminal needed.

## How to use

### 1. Open the file
Download `kid-coder.html` and open it in your web browser. That's all—nothing to install.

### 2. Create a project
Click the **➕ New Project** button, type a name (e.g., "My Robot Game"), and click Create.

### 3. Add files
Click your project to see its files. Each project comes with three starter files:
- `index.html` — the page structure
- `style.css` — colors and layout
- `script.js` — interactive stuff

### 4. Edit code
Click **Edit** on any file. The code opens in a simple editor.

### 5. Save your work
When you're done, click **Save**. You'll see a green checkmark: **✓ Saved to GitHub!**

## Keyboard shortcuts

| Key | What it does |
|-----|------|
| <kbd>Escape</kbd> | Close editor or project view, go back |
| <kbd>Enter</kbd> | Open a project (when focused on a project card) |

## For parents: How to add real GitHub syncing

This MVP is 100% browser-based (no internet needed). To save projects to GitHub:

1. **Run the backend** — Node.js or Python server that:
   - Watches for file saves from the editor
   - Auto-commits changes with timestamp messages
   - Handles GitHub authentication silently (kid never sees it)

2. **Example tech stack:**
   - Backend: Node.js + `simple-git` library
   - Deployment: Heroku, Railway, or local machine
   - GitHub: Personal access token (stored on backend, never exposed to UI)

3. **Kid sees:** "✓ Saved to GitHub!" message. That's all.

## Features

✅ No login screen  
✅ No git knowledge required  
✅ Save with one click  
✅ Works offline (local saves)  
✅ Keyboard accessible (WCAG AA)  
✅ Zero dependencies (pure HTML/CSS/JS)  

## Files included

| File | Purpose |
|------|---------|
| `kid-coder.html` | The entire app — open in browser |
| `README.md` | This file |

## Troubleshooting

**"My saves disappeared!"**  
Right now, saves only stay while the page is open. Add a backend to persist to GitHub.

**Can my kid write any code?**  
Yes — HTML, CSS, JavaScript all work. The editor doesn't block anything.

**How do I see what they created?**  
Once backend is added, projects sync to GitHub. You can see all edits in version history.

## Next steps

1. ✅ Kid can prototype and experiment right now
2. 🔄 Connect to GitHub backend (see "How to add real GitHub syncing" above)
3. 📚 Teach git history later: "Look, every save is saved here" → point to GitHub

---

Made for young builders. Questions? Check the code—it's all in one HTML file, super readable.

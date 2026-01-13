# PLM - Psyop Language Model

Dark, stormy AI chatbot. Two-page site with character-focused design.

## Structure

```
plm-site/
├── index.html         ← Landing page (hero with PLM character)
├── chat.html          ← Chat terminal (character visible on left)
├── api/
│   └── chat.js        ← Backend (calls Claude API)
├── plm-character.png  ← Your character image
├── vercel.json
└── package.json
```

---

## Deploy to Vercel (10 min)

### 1. Add your character image
Name it `plm-character.png` and put it in the root folder.

### 2. Push to GitHub
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin YOUR_REPO_URL
git push -u origin main
```

### 3. Deploy
- Go to [vercel.com](https://vercel.com)
- Import your repo
- Deploy

### 4. Add API Key
- Project Settings → Environment Variables
- Add: `ANTHROPIC_API_KEY` = your key
- Redeploy

---

## Customize

### X (Twitter) Link
In `index.html`, find:
```html
<a href="#" class="x-link"
```
Change `href="#"` to your X URL.

### Pump.fun / Token Links
Add wherever you want in the HTML.

### Colors
Edit CSS variables at top of each HTML file:
```css
--red-primary: #d62828;
--red-glow: rgba(214, 40, 40, 0.6);
```

---

## Pages

**/** — Landing page with PLM standing, "ENTER TERMINAL" button

**/chat.html** — Chat interface with PLM visible on the left side

---

$PLM • Nothing is organic • Trust no one

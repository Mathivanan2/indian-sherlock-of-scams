# Indian Sherlock of Scams

A hobby blog investigating financial crime, banking fraud, and AI scams — written like detective case files.

This is a plain HTML/CSS/JS site. No build tools, no npm install, no server required. You can deploy it for free and it will just work.

---

## 1. Going live for the first time

**Step 1 — Create a GitHub account** (if you don't have one): https://github.com

**Step 2 — Create a new repository**
- Click "New repository"
- Name it something like `indian-sherlock-of-scams`
- Keep it Public
- Don't add a README/gitignore (you already have files)

**Step 3 — Upload these files**
- Open your new repo on GitHub → click "Add file" → "Upload files"
- Drag in the entire contents of this folder (keep the `posts/` and `assets/` folders intact)
- Commit the changes

**Step 4 — Connect to Netlify**
- Sign up free at https://netlify.com using your GitHub account
- Click "Add new site" → "Import an existing project" → choose your repo
- Build settings: leave everything blank/default (this is a static site, nothing to build)
- Click "Deploy"
- Within a minute you'll get a live URL like `https://random-name-123.netlify.app`

**Step 5 (optional) — Custom domain**
- Buy a domain (Namecheap, GoDaddy, Google Domains — around $10-15/year)
- In Netlify: Site settings → Domain management → Add custom domain
- Follow the DNS instructions Netlify shows you

**Step 6 — Turn on the contact/subscribe forms**
- Netlify auto-detects forms with `data-netlify="true"` (already set up on `contact.html` and the homepage subscribe box)
- Go to Site settings → Forms in your Netlify dashboard to see submissions — no extra setup needed

---

## 2. Posting a new blog (your regular routine)

**Step 1 — Duplicate the template**
- Copy `posts/post-template.html`
- Rename it something like `posts/case-file-02-the-fake-loan-app.html`

**Step 2 — Write your story**
- Open the new file in any text editor (even Notepad works)
- Replace everything in `[square brackets]` with your actual content
- Keep the HTML tags (`<h2>`, `<p>`, etc.) as they are — just change the text inside them

**Step 3 — Add it to the Stories page**
- Open `stories.html`
- Copy one of the existing `<a class="pin">...</a>` blocks
- Update the link, badge, title, description, and category tag

**Step 4 — Add it to the homepage (optional)**
- Open `index.html`, update the "Latest case files" section the same way

**Step 5 — Update the RSS feed**
- Open `rss.xml`, copy an `<item>` block, update it for your new post

**Step 6 — Upload and go live**
- On GitHub: go to your repo → navigate to the `posts` folder → "Add file" → "Upload files" → drop in your new file → Commit
- Also re-upload `stories.html`, `index.html`, and `rss.xml` since you edited them (same Upload files process, GitHub will overwrite the old versions)
- Netlify auto-detects the change and rebuilds your site within about a minute — no extra step needed

---

## 3. Security checklist

- [ ] Enable 2FA on your GitHub account
- [ ] Enable 2FA on your Netlify account
- [ ] Enable auto-renewal + domain lock if you buy a custom domain
- [ ] Only add third-party scripts/widgets from reputable, well-known services
- [ ] HTTPS is automatic on Netlify — just confirm it's showing the padlock once live

---

## File structure

```
/
├── index.html          → Homepage
├── stories.html         → Case file archive
├── about.html            → About the author page
├── contact.html         → Contact + tip line form
├── rss.xml                    → RSS feed (update when you post)
├── styles.css              → Shared site-wide styles
├── posts/
│   ├── case-file-01.html      → Sample post (HSBC impersonation scam)
│   └── post-template.html     → Copy this for every new post
└── assets/
    ├── logo.svg               → Full logo with wordmark
    └── logo-icon.svg           → Icon-only logo (favicon, social)
```

---

## Notes

- This blog is educational only — every post includes a disclaimer at the bottom. Keep that in place on new posts.
- When writing about real companies or institutions, only describe them as the *target* of impersonation scams (like the HSBC example), never as the perpetrator — this keeps content accurate and safe to publish.

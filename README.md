# Mayuri T — Portfolio

A single-page portfolio built with plain **HTML, CSS, and vanilla JavaScript** — no build step, no npm install required.

## Run it in VS Code

1. Unzip/open this `portfolio` folder in VS Code.
2. Install the **Live Server** extension (by Ritwick Dey) if you don't have it.
3. Right-click `index.html` → **Open with Live Server**.
   - Or just double-click `index.html` to open it directly in a browser (some effects like the canvas background still work fine).

## Structure

```
portfolio/
├── index.html      # all content/sections
├── style.css        # design system: colors, type, layout, animations
├── script.js         # typing effect, scroll reveals, filters, canvas bg, theme toggle
└── assets/
    ├── mayuri.jpg          # your photo
    └── Mayuri_Resume.pdf   # your résumé (linked to the "Download Résumé" button)
```

## What's real vs. what to double-check

Everything in this site is pulled directly from your resume — CGPA, internship, all 4 projects, certifications, and skills. Nothing was invented. Before you publish it:

- **Update LinkedIn/GitHub links** — currently placeholder `#` links in the Contact section (search for `class="social-link"` in `index.html`).
- **Contact form** — it's front-end only right now (it just shows a confirmation message). To actually receive messages, wire it to a service like Formspree, EmailJS, or a small backend/Supabase function.
- **Project visuals** — each project card uses a simple generated SVG icon instead of a screenshot. Swap in real screenshots of your Excel dashboard, the Expense Tracker UI, etc. for more impact — replace the `.project-visual` block in `index.html` with an `<img>` tag.

## Customizing

- **Colors/fonts**: edit the `:root` variables at the top of `style.css`.
- **Typing animation phrases**: edit the `roles` array in `script.js`.
- **Add a project**: copy one `<article class="project-card" data-tags="...">` block in `index.html` and edit the text/tags.

## Deploying

Free and simple: drag the `portfolio` folder into [Netlify Drop](https://app.netlify.com/drop), or push it to a GitHub repo and enable **GitHub Pages** in the repo settings.

# Lakshya Mishra: Portfolio

Personal portfolio of an AI/ML and software engineer. A static site (HTML, CSS, vanilla JS), no build step.

## Highlights
- Kinetic name hero, hover-reveal project list with metric previews
- Interactive **alert triage demo**: an illustrative replay of a multi-agent security pipeline (detector, supervisor, specialist agents, safety layer, human approval)
- In-page resume viewer plus a PDF download
- Contact form (Formspree), light and dark theme, mobile friendly

## Structure
```
index.html     page markup
styles.css     styles and theme tokens
script.js      demo, hover previews, resume viewer, contact form
assets/        photo.jpg, resume.jpg (image shown in the viewer)
resume.pdf     downloadable resume
```

## Run locally
```
python3 -m http.server 8000
```
Then open http://localhost:8000.

## Deploy on Vercel
Import the repo in Vercel, choose "Other" as the framework preset, leave the build command empty and the output directory as the root.

## Make it yours
- **Contact form:** create a form at https://formspree.io and paste its URL into `FORM` at the top of the contact section in `script.js`. Without it, the form falls back to a `mailto:` link.
- **Resume:** replace `resume.pdf`, and re-export its first page as `assets/resume.jpg` (the in-page viewer shows this image).
- **Headline project:** "Alert Triage Agents" is a working title with no evaluation metrics yet. Update the name and numbers in `index.html` once final.
- **Demo data:** the triage demo uses illustrative sample alerts defined in `script.js`; it does not process live traffic.

# Shashankh Varma Vegesna, portfolio

A single static page (index.html). No build step.

## Run it locally (VS Code)
Open this folder in VS Code and run `npx serve .` in the terminal, then open the
address it prints. Opening index.html directly in a browser also works.

## Deploy on Netlify
Option A: go to app.netlify.com/drop and drag this whole folder onto the page.
Option B: push this folder to a GitHub repo, then in Netlify choose
"Add new site > Import an existing project", pick the repo, leave the build command
empty and set the publish directory to `.` (netlify.toml already says this).

## After you have your final address
1. In index.html, add inside <head>:
   <link rel="canonical" href="https://YOUR-ADDRESS/"> and
   <meta property="og:url" content="https://YOUR-ADDRESS/">
2. Add `Sitemap: https://YOUR-ADDRESS/sitemap.xml` to robots.txt if you add a sitemap.

## Add your LinkedIn, GitHub and portfolio links
In index.html, search for `links:{linkedin:"",github:"",portfolio:""}` and paste
your URLs between the quotes. Buttons appear only for links you fill in.

## Notes
- Off claude.ai, the AI guide, demo and Fit Lab use their built-in, in-browser logic
  (no API key needed). To use a hosted model, put your endpoint URL in
  <meta name="guide-endpoint" content="">.
- The résumé PDF is embedded in the page; a copy is in assets/.
  Its source is source/resume.html.
- Sound is off until a visitor turns it on. No phone number appears anywhere.

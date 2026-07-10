# Custom Portfolio — Setup Guide

This is a custom single-page site (like Nate's) that REPLACES the lowinertia template.
It uses the same GitHub Pages hosting and the same URL: ellaclek.github.io

## What's in this zip
- index.html ............ the entire website (one file)
- .nojekyll ............. tells GitHub Pages to serve the HTML as-is
- projects/built-on-truss/ .. the project images used on the page

## The big picture
Your repo currently holds the template's files (_config.yml, _projects, etc.).
We're going to clear those out and put these files in instead. Your repo name and
URL don't change — only the contents.

------------------------------------------------------------------------
## OPTION A — Cleanest (recommended): fresh start in the same repo
------------------------------------------------------------------------

Because there are many template files to delete one-by-one in the browser, the
simplest reliable path is to delete the repo and recreate it empty, then upload
these files. Your URL stays identical.

1. Go to github.com/ellaclek/ellaclek.github.io
2. Settings (top tab) → scroll to the very bottom → "Delete this repository"
   - Follow the prompts (you'll type the repo name to confirm)
   - This is safe: everything we made is saved in this zip
3. Create it again: top-left "+" → New repository
   - Repository name: ellaclek.github.io  (exactly, same as before)
   - Public, and check "Add a README" so the repo isn't empty
   - Create repository
4. Upload these files:
   - On the repo page: "Add file" → "Upload files"
   - From this zip, drag in: index.html, .nojekyll, and the whole projects folder
     (drag the projects FOLDER itself so the images keep their path)
   - If the browser won't accept the folder, do this instead:
       a. Upload index.html and .nojekyll first, commit
       b. "Add file" → "Create new file", name it:
          projects/built-on-truss/placeholder.txt  → type "x" → commit
       c. Go into projects/built-on-truss, "Add file" → "Upload files",
          drag all the .jpg files in, commit
5. Settings → Pages → Source = "Deploy from a branch", branch = main, folder = / (root)
6. Wait 2–3 minutes, visit https://ellaclek.github.io

------------------------------------------------------------------------
## OPTION B — Keep the repo, swap the files
------------------------------------------------------------------------

If you'd rather not delete the repo:
1. In the repo, delete these template items (each: click it → ... menu or trash icon → commit):
   _config.yml, index.md (or index.html if present), _projects, _layouts,
   _includes, _sass, assets, Gemfile, and any other template files EXCEPT .git
2. Then follow Option A steps 4–6 to upload these files.

Option A is genuinely less work because deleting files one-by-one in step 1 here
is tedious.

------------------------------------------------------------------------
## After it's live
------------------------------------------------------------------------
- Résumé button: currently points to /assets/resume/resume.pdf. Upload your resume
  there (create the folders via "Create new file" → assets/resume/resume.pdf won't
  work for a PDF upload, so: Add file → Upload files, drag resume.pdf, then rename
  the path to assets/resume/resume.pdf), OR tell me a Google Drive link and I'll
  wire it in.
- Everything else (email, phone, LinkedIn, GitHub) is already filled in.

## Adding a project later
Open index.html, find the "PROJECTS" section, copy one <article class="proj"> block,
paste it below, and edit the text + image paths. Send me the details and I'll do it
for you.

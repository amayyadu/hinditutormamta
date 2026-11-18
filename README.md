Hindi with Mamta

Website for Mamta Rani's online Hindi lessons. A single static page (index.html) with no build step.

Editing content

Open index.html and look for the block marked EDIT HERE: site settings and course content (search for var CFG). Course names, blurbs, the announcement bar, contact email and photo filenames are all there. The Terms and Privacy pages are plain HTML inside the same file (search for data-view="terms" and data-view="privacy").

Photos

Put the photos in the same folder as index.html, named as in CFG: mamta-teacher.jpg and mamta-portrait.jpg.

Publishing changes

The site is hosted on Netlify, connected to this repository. Commit and push to main and Netlify redeploys automatically within a minute.

git add .
git commit -m "Describe what you changed"
git push
Notes
Form submissions and student accounts use Supabase. The key in index.html is a publishable key, which is meant to be public, but only if Row Level Security is switched on for every table.
Update the "Last updated" date at the top of the Terms and Privacy pages when you change them.

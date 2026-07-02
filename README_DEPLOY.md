# Chronos Project Page Deployment Guide

This package follows a ContactWorld-style independent GitHub Pages setup.

## 1. Create a short-domain GitHub Pages repository

Recommended organization name:

- chronos-manipulation

Then create a public repository under that organization named exactly:

- chronos-manipulation.github.io

The final website will be:

- https://chronos-manipulation.github.io/

If the organization name is different, the repository must be named:

- <organization-name>.github.io

## 2. Upload this package to the repository root

The repository root should contain:

- index.html
- .nojekyll
- static/css/style.css
- static/images/
- static/videos/

Do not put these files under docs/ for this short-domain setup.

## 3. Prepare images

Place the following images:

- static/images/framework.png
- static/images/results.png

Optional:
- You can replace sections or add more figures later.

## 4. Prepare videos

Place the following exact video filenames into static/videos/:

- ALOHA_DIFFUSION.mp4
- ALOHA_SB.mp4
- rw1_pi05.mp4
- rw1_chronos.mp4
- rw2_pi05.mp4
- rw2_chronos.mp4
- rw3_pi05.mp4
- rw3_chronos.mp4
- rw4_pi05.mp4
- rw4_chronos.mp4
- rw4-2.mp4
- rw4-3.mp4

Filenames are case-sensitive on GitHub Pages.

## 5. Local preview

Run this command in the website repository root:

python -m http.server 8000

Then open:

http://localhost:8000

## 6. Push to GitHub

git add .
git commit -m "Launch Chronos project page"
git push origin main

## 7. Enable GitHub Pages

Go to:

Repository -> Settings -> Pages

Set:

Source: Deploy from a branch
Branch: main
Folder: /root

The website should appear after several minutes.

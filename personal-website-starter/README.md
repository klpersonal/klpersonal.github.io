# Personal Website Starter

A simple academic/professional personal website built with Jekyll and designed
for GitHub Pages.

## Pages included

- Home
- About
- Publications
- CV
- Blog
- Example blog post

## 1. Customize the content

Replace `Your Name`, the biography, publications, positions, links, and other
placeholder text throughout the files.

Put your actual CV PDF at:

    assets/files/cv.pdf

## 2. Add a blog post

Create a Markdown file in `_posts` named:

    YYYY-MM-DD-title.md

Example:

    2026-09-01-my-new-paper.md

At the top:

    ---
    layout: post
    title: "My new paper"
    ---

Then write the post in Markdown.

## 3. Test locally (optional)

Install Ruby and Bundler, then run:

    bundle install
    bundle exec jekyll serve

Open the local address printed in the terminal.

## 4. Publish with GitHub Pages

For a personal site, create a GitHub repository named:

    YOUR-USERNAME.github.io

Upload or push these files to the repository.

In GitHub:

Settings > Pages > Build and deployment

Choose:

- Source: Deploy from a branch
- Branch: main
- Folder: /(root)

GitHub will publish the site at:

    https://YOUR-USERNAME.github.io

## 5. Optional custom domain

Buy a domain such as `yourname.com`, then configure it under:

Settings > Pages > Custom domain

Follow GitHub's DNS instructions for your domain provider.

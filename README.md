# Roland Andrews – Personal Website

This repository contains a **very simple, fully static personal website**.  
It is meant as a clean starting point to present research, projects, and a small blog without any build tools or frameworks.

## Structure

- `index.html` – main page with sections for About, Research, Blog, and Contact.
- `assets/css/main.css` – shared styling (typography, layout, light theming).
- `posts/example-post.html` – example blog post you can copy when creating new posts.

Everything is plain **HTML + CSS**. There is a tiny inline script only to keep the year in the footer up to date.

## Running locally

No special setup is required:

- **Option 1 (simplest)**: Just open `index.html` in your browser.
- **Option 2 (nicer URLs)**: Serve the folder with any static file server, for example:

```bash
cd /path/to/RolandAndrews.github.io
python -m http.server 8000
```

Then open `http://localhost:8000` in your browser.

## Customizing the site

Edit these parts to make it yours:

- **Name & tagline**: Update the header in `index.html` (the “Roland Andrews” text and description).
- **About section**: Replace the placeholder paragraphs under the `#about` section.
- **Research cards**: In the `#research` section, change titles/descriptions and add or remove cards.
- **Contact info**: Update email, GitHub handle, and any other links in the `#contact` section.

### Adding blog posts

1. Copy `posts/example-post.html` to a new file, e.g. `posts/my-first-post.html`.
2. Change the `<title>`, `<h1>`, meta text, and content in the new file.
3. In `index.html`, inside the **Blog** section, add a new list item linking to your new post:

```html
<li class="post-card">
  <h3><a href="posts/my-first-post.html">My first post</a></h3>
  <p class="post-meta">Date or short meta text</p>
  <p class="post-excerpt">One or two sentences describing the post.</p>
</li>
```

You can keep everything this simple, or later introduce a generator (like Jekyll) if you decide you need it.



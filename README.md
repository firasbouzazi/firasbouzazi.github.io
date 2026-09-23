# firasbouzazi.github.io

A minimalist, static blog. No framework, no build step, no tracking.

## Structure

```
index.html        Home: bio line + list of posts
style.css         The whole design system (light + dark)
theme.js          Light/dark toggle, remembered per reader
posts/            One HTML file per article
  _template.html  Copy this to start a new post
```

## Adding a post

1. Copy `posts/_template.html` to `posts/your-slug.html`.
2. Fill in the title, date, and prose. The `.prose` container styles
   `h2`, `h3`, `p`, `ul`/`ol`, `blockquote`, `code`, `pre`, and `figure`.
3. Add an entry to the `<ul class="posts">` list in `index.html`, newest first:

   ```html
   <li>
     <a class="entry" href="posts/your-slug.html">
       <span class="entry-title">Your title</span>
       <span class="entry-date">YYYY-MM-DD</span>
       <p class="entry-desc">One-line description.</p>
     </a>
   </li>
   ```

That's it. Commit and push.

## Branches

- `main`: this blog (published via GitHub Pages).
- `legacy`: the previous neon CV site with the interactive game.

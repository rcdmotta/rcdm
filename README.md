# Ricardo Motta – personal website

A static website written in plain HTML, CSS and a little JavaScript, with no frameworks
and no build step. It recreates the Google Site <https://sites.google.com/view/ricardomotta/>
and is published with GitHub Pages.

## Files

| Path | Contents |
|---|---|
| `index.html` | Home page |
| `talks-and-events.html` | Talks and events page |
| `assets/css/style.css` | All styling; the colours are defined at the top |
| `assets/js/main.js` | Opens and closes the menu on phones |
| `assets/images/` | Banner photo (used on every page) and profile photo |
| `assets/fonts/` | Bitter and Open Sans font files, with their licences |
| `.nojekyll` | Tells GitHub Pages to publish the files exactly as they are |

## Editing

- **Text:** open the `.html` file in any text editor and change the text between the tags.
- **New event:** in `talks-and-events.html`, copy one `<li>…</li>` line and edit it.
  `class="os"` gives the font Open Sans; leave it out to use Bitter.
- **New page:** copy `talks-and-events.html` to a new name, change its title and content,
  then add `<li><a href="new-page.html">New page</a></li>` to the menu (`<nav class="menu">`)
  in every page. Mark the current page's menu link with `aria-current="page"`.
- **Preview:** open `index.html` in a browser (double-click), or run a local web server in this folder.

## Presentations and other self-contained material

Give each one its own subfolder, for example `talks/2026-example/index.html`, with all its files
inside that subfolder. Link to it with a relative path such as `talks/2026-example/`.

## Publishing

Commit and push to the `main` branch. GitHub Pages republishes the site automatically,
usually within a minute or two.

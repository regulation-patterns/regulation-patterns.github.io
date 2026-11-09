# Regulation Patterns website

This repository is public and builds https://regulation-patterns.github.io: the Pattern List (/pattern-list/) and the
Pattern Atlas (/pattern-atlas/), moved here from the Metabolism Regulation website on 2026-11-08 (user), same
addresses, hidden for now (`noindex` on every page).

Page code only. What the pages show (`_pattern_maps/`, `pattern-atlas-downloads/`, `atlas-data/`, `_data/pattern_*.csv`)
is kept in a private repository and put in only when the site is built (`.github/workflows/build.yml`, one secret,
`DATA_TOKEN`). They are ignored here (`.gitignore`); never commit them. The lists, maps and texts are made in a
private repository whose copy script writes them into the data; change them there.

Names: this repository is public and names no private repository, in files, pages, code comments or commit messages.

- The viewer (`_includes/atlas-app.html`, `atlas-tags.css`) is a copy of the viewer's one source (since 2026-11-10,
  user; `_includes/VERSION` names its commit), taken again only when the user asks. The Pattern Atlas has the look
  Default Lines of the viewer's styles page in presentation mode, top bar kept (user, 2026-11-10):
  `_includes/default-lines.css`, a copy of that style, included before the viewer, which gets `look="version1"` (the
  base the style was made on). The layouts and styles are copies of the Metabolism Regulation website's (2026-11-08).
- One top bar (`_data/mastheads.yml`, `masthead: patterns`): no logo, the site's name, Pattern Atlas then Pattern List;
  the page shown not in bold (`plain: true`, user 2026-11-10).
- The page text of the Pattern List is edited here (`pages/pattern-list.md`).
- After the data change, the workflow is started by hand or by the session that pushed them; a push here starts it too.
- A change counts only when it is live, checked on the site itself.

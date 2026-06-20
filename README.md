# SMSN Toolkit for Accessible Maths

A Jekyll-based website styled with [Bulma](https://bulma.io), built to run on
GitHub Pages, and to be easily editable.

## The most common edits

**Add or change an external link** — edit `_data/links.yml` (for the External Links page).
Each entry is just:

+ a title, 
+ a url and 
+ a description.

**Add or change an entry in the Toolkit Hub** -- edit `_data/toolkit.yml` (for the Toolkit Hub page).
Each entry is just:
+ a title, 
+ a url and 
+ a description.

Copy an existing block and change the text. No HTML involved.

**Edit page text** — open the relevant `.md` file in the root folder
(`index.md`, `purpose.md`, `contact.md`, etc.) and edit the text below the
`---` front matter block at the top. Leave the front matter itself alone.

**Add a whole new page** — create a new `.md` file in the root folder with
front matter like:

```yaml
---
layout: default
title: Page Name
permalink: /page-name/
---
```

then add a matching entry to `nav_pages` in `_config.yml` so it shows up
in the navigation bar.

**Change colors or fonts** — edit the variables at the top of
`assets/css/custom.css`. Bulma itself (loaded from a CDN in
`_layouts/default.html`) never needs to be touched.

## Structure

```
_config.yml             site title, description, and nav order
_layouts/default.html   the one page template every page uses
assets/css/custom.css   colors, fonts, hover effects
_data/toolkit.yml       content for the Toolkit Hub page
_data/links.yml         content for the External Links page
index.md                Toolkit Homepage (splash screen)
purpose.md              Purpose
toolkit-hub.md          Toolkit Hub — the main starting point for using the toolkit
external-links.md       External Links
contact.md              Contact
```

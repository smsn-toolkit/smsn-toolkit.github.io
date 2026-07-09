# Materials Directory

This directory contains self-contained resources: standalone HTML slidedecks, complete websites, and other pre-built materials that are to be linked from the main toolkit pages.

## How to add a resource

1. **Create a subdirectory** for your resource under `materials/`. Use a short, descriptive name with no spaces (e.g., `quarto-workshop-jan-2026`).

2. **Place all files in that subdirectory**:
   - For single HTML slidedecks: put `index.html` (or your filename) directly in the folder.
   - For complete site with assets (in a subfolder): fine to dump `html` files and further subfolders here.

As long as the main file is called `index.html` it will be found automatically by pointing to just the folder below.

3. **Link to it** in `_data/toolkit.yml` or `_data/links.yml`:
```yaml
   - title: Resource Title
     url: /materials/resource-name/
     description: Brief description of what this resource contains.
```

If the file is not called `index.html`, e.g. it's called `slides.html` then you'll need to point directly to it in the `url` link above and not just end with `/`.


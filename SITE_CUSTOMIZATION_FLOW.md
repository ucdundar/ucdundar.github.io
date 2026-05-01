# Site Customization Flow

## Fast Map

`Change homepage bio/photo`
-> `_pages/about.md`
-> image file in `assets/img/`

`Change contact / social links`
-> `_data/socials.yml`

`Change publications`
-> `_bibliography/papers.bib`

`Change CV page`
-> `assets/json/resume.json`
-> optional PDF in `assets/pdf/`
-> link button in `_pages/cv.md`

`Change top navigation`
-> any file in `_pages/`
-> set `nav: true/false`
-> set `nav_order`

`Add a new page`
-> copy an existing file in `_pages/`
-> set:
   - `title`
   - `permalink`
   - `nav: true`
   - `nav_order`

`Add downloadable files`
-> put file in `assets/files/`
-> link it from a page with:
-> `/assets/files/your-file-name.xlsx`

`Update thesis supervision topics`
-> edit `_data/thesis_topics.yml`
-> change `status: open|reserved|completed`
-> page updates automatically

`Use Google Sheets for thesis topics`
-> publish sheet to web
-> copy embed URL
-> paste into `google_sheet_embed` in `_pages/thesis-supervision.md`

## Example: Bachelor Thesis Supervision Page

1. Edit `_pages/thesis-supervision.md`
2. Replace the placeholder text
3. Replace `assets/files/bachelor-thesis-topics.csv`
4. If you want Excel instead:
   - add `assets/files/bachelor-thesis-topics.xlsx`
   - change the link in `_pages/thesis-supervision.md`

## Update Loop

`Edit content`
-> `save file`
-> `check page locally or on GitHub Pages`
-> `commit`
-> `push`

## Files To Ignore Unless Needed

- `_layouts/`
- `_includes/`
- `_sass/`
- `_plugins/`

Only touch those if you want design/layout changes rather than content changes.

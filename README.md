# SEMICON Sponsors Logo HTML Generator

A browser-based HTML generator for maintaining SEMICON Taiwan sponsor logo sections and producing Drupal-ready bilingual HTML.

Current version: **v5.1.1**

## Purpose

Sponsor logos often arrive in batches and change over time. This tool helps editors maintain the current sponsor output list, check whether logos are ready, preview the result, and copy production-ready HTML for Drupal without editing code manually.

## Key Features

- Sponsor logo upload, paste, and drag-and-drop input
- Sponsor tier grouping: Platinum, Gold, Silver, Special
- Inline sponsor link editing
- Logo display scale adjustment
- Drag-and-drop sponsor ordering
- Chinese and English HTML output
- Desktop and mobile preview
- Preview language switch
- Local auto-save in the browser
- Work file export/import for handover
- Automatic readiness status:
  - `Ready`: logo and sponsor name are present
  - `Check`: publishable but missing a name or link
  - `Missing`: missing required logo image
- Status summary, for example:
  - `4 logos · 2 ready · 0 missing · 2 check`

## Usage

1. Open `index.html` in a browser or through the GitHub Pages deployment.
2. Add sponsor logos by uploading, pasting, or dragging image files into the logo area.
3. Choose the sponsor tier and add the sponsor name and URL when available.
4. Review the sponsor list and status labels.
5. Adjust logo scale or sponsor order if needed.
6. Open the preview tab and choose Chinese or English preview.
7. Copy the Chinese or English HTML into the corresponding Drupal content area.
8. Use `Save work file` to keep a JSON work file for future updates.

## Work File

The work file is a JSON backup for long-running sponsor updates. It includes:

- Schema name
- Tool name
- Tool version
- Project name
- Export timestamp
- Sponsor data
- Tier title settings

Use `Load work file` to continue editing a previously exported work file.

## Important Notes

- The generated HTML is designed for direct Drupal usage.
- Browser auto-save uses `localStorage`, so it is tied to the same browser and URL.
- Use `Save work file` before switching devices, clearing browser data, or handing work to another editor.
- Do not commit private sponsor assets or unpublished internal content unless approved.

## Version History

### v5.1.1

- Added publish readiness signal: `Needs attention` / `Ready to publish`
- Added visible reason text for `Check` status
- Renamed import action to `Load work file`
- Added sample data warning after loading sample sponsors

### v5.1

- Added status summary counts
- Added automatic sponsor status labels
- Added empty state and sample data
- Added work file metadata
- Added Chinese / English preview switch

### v5.0

- Added inline editing and backup/restore workflow

# Talabat Updates Board

A single-file, browser-based updates board for the Talabat Menu Auditing team. It is designed to run as a static site on GitHub Pages with no build step and no backend.

## Run locally

Open `index.html` in a modern browser, or serve the folder with any static web server. For example:

```bash
python3 -m http.server 8000
```

Then open <http://localhost:8000>.

## Publish with GitHub Pages

1. Create a GitHub repository and upload `index.html` and this `README.md`.
2. In the repository, open **Settings → Pages**.
3. Select **Deploy from a branch**, choose the default branch and `/ (root)`, then save.
4. GitHub will provide the published Pages URL.

## Important data note

Updates, links, author name, and attached images are stored in the browser's `localStorage`. That means each browser/device has its own copy; publishing the file on GitHub does not create a shared database. Clearing browser data can remove the locally saved content.

## Suggested next improvements

- Add a small backend or hosted database if multiple auditors must see and edit one shared live board.
- Add user authentication and per-user permissions before storing operational content centrally.
- Add optimistic conflict handling or revision history so simultaneous edits are not lost.
- Add structured fields such as owner, priority, status, due date, and tags to improve search and reporting.
- Add automated tests for adding, editing, deleting, pinning, searching, and link management.
- Consider self-hosting the fonts if the board must work without third-party network requests.

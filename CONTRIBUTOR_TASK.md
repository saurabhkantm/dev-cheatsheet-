# Contributor Task Document

## Project Overview

**PROJECT NAME:** Dev Cheatsheet

**REPO:** https://github.com/rabbikazmi/dev-cheatsheet-

Dev Cheatsheet is a fast, simple, lightweight reference tool for developers to quickly look up and copy common code snippets. It is built with vanilla HTML, CSS, and JavaScript — no frameworks or build tools required.

**Tech Stack:**
- Frontend: Vanilla HTML, CSS, JavaScript (no frameworks)
- Backend: None (fully static)
- Database: None (data stored in data.js)
- Other Tools: None

**Current Features:**
- Real-time search by title or description
- Filter by category (Git, Terminal, JavaScript, CSS)
- One-click copy to clipboard
- Responsive design (desktop, tablet, mobile)
- No dependencies, ~100KB total
- Easy to extend by editing data.js

**Target Users:** Developers (beginner to intermediate) who want a quick offline/local cheatsheet reference without any setup.

---

## File Structure

```
index.html       - Main HTML page
style.css        - All styling
script.js        - Search, filter, copy functionality
data.js          - Array of cheatsheet objects
CONTRIBUTING.md  - Contribution guidelines
README.md        - Project documentation
```

---

## Architecture / Key Modules

- **data.js** → `/data.js` → Stores all cheatsheet entries as a JS array of objects
- **script.js** → `/script.js` → Handles search, filtering, rendering cards, copy-to-clipboard
- **style.css** → `/style.css` → All visual styling, responsive layout
- **index.html** → `/index.html` → Entry point, loads all files, renders the page structure

---

## Getting Started / Setup

**Prerequisites:** Any modern browser, Git

**Installation:**
1. No installs needed
2. Clone the repo: `git clone https://github.com/rabbikazmi/dev-cheatsheet-.git`
3. Open `index.html` in your browser

**Adding a Cheatsheet:**
1. Edit the `cheatsheetData` array in `/data.js`
2. Add a new object with: `{ title, category, description, code }`

**Notes:**
- No environment variables
- No database setup
- No build step required

---

## New Feature Ideas

1. **Dark Mode Toggle** (Beginner, ~4-6 hours)
   - Affects `style.css` and `script.js`

2. **New Category Support: Python / React / Docker** (Beginner, ~2-3 hours)
   - Affects `data.js` and `index.html` filter buttons

3. **Bookmark / Favorites Feature** (Intermediate, ~8-10 hours)
   - localStorage to save favorites
   - Affects `script.js` and `style.css`

4. **Export Cheatsheets as PDF** (Intermediate, ~10-12 hours)
   - Use a library like jsPDF
   - Affects `script.js` and adds a new button in `index.html`

---

## Good First Issues

1. Add loading spinner or skeleton card while cheatsheets render
2. Add "No results found" empty state message when search returns nothing
3. Improve README with screenshots of the UI
4. Add a "Back to Top" button for long scroll
5. Fix any inconsistent button hover styles in `style.css`
6. Add a new cheatsheet entry to `data.js` (e.g., a Markdown or Regex cheatsheet)

---

## Already Open Issues

Several issues are already opened and ready for contribution:

1. **Layout breaks on mobile devices (not responsive)** (#11)
   - Affects responsive design on small screens
   
2. **Add a new tool/language category** (#8)
   - Enhancement to expand cheatsheet categories
   
3. **Add more cheatsheets to an existing category** (#7)
   - Help expand the cheatsheet library
   
4. **Add an "All" filter button that is active by default** (#6)
   - Improve filtering functionality
   
5. **Make the category filter buttons scrollable on mobile** (#5)
   - Mobile UX improvement
   
6. **Make the search bar clear with an X button** (#3)
   - Quality of life feature
   
7. **Add card count below the search bar** (#2)
   - Display improvement
   
8. **Add a "copy" success animation on the copy button** 
   - UX enhancement for feedback

Check the [GitHub Issues](https://github.com/rabbikazmi/dev-cheatsheet-/issues) page for the latest updates and to claim an issue to work on.

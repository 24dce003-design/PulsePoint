# These Fitness — Website README

This README documents the "These Fitness" student website in this workspace. It explains the project structure, how to run and test the site locally, how to customize content, and tips for producing screenshots/PDFs for submission.

If you want this to be the repository README shown by GitHub or your editor, rename the file to `README.md`.

Project overview
----------------
These Fitness is a small responsive website that provides fitness-related pages: workouts, nutrition, membership, recipes, and sample interactive pages. The site is built with plain HTML, CSS and JavaScript so it can be run locally without a server. Some pages may call PHP endpoints if you added server-side features — check the files for `.php` references.

Quick start — open in your browser
---------------------------------
1. Open the project folder: `C:\Users\adroj\OneDrive\Desktop\HTML2`
2. Double-click the HTML file you want to preview (for example `workout2.html` or `nutrition2.html`). The file will open in your default browser.

Serve with a simple local web server (recommended)
-------------------------------------------------
Using a simple HTTP server avoids some browser restrictions (CORS, module imports) and matches how the site will behave when hosted.

- Python 3 (PowerShell):

```powershell
cd 'C:\Users\adroj\OneDrive\Desktop\HTML2'
python -m http.server 8000
# then open http://localhost:8000/workout2.html
```

- VS Code: install the Live Server extension and use "Open with Live Server" on any HTML file.

Project file map (key files)
----------------------------
- `first2.html`, `first2.js` — a demo/sample page (might be your starting page)
- `workout2.html`, `workout2.js` — workout page + interactive scripts
- `nutrition2.html`, `nutrition2.js` — nutrition page + scripts
- `recipes2.html`, `recipes2.js` — recipes browsing and interactivity
- `membership2.html`, `membership2.js` — membership form or flow
- `login2.html`, `login2.js` — login demo (client-side)
-  `bmicalculator2.*`, `liveclass2.*` and other HTML/JS are additional pages in the workspace.
- `php/` — optional: server-side PHP files if present (for example `menu.php` in other projects). If you have PHP endpoints, run via XAMPP or another PHP-enabled server.
- `LOGO.png`, `header.jpeg`, `images.jpeg` — image assets (useful for headers and cards)

Features to check and test
--------------------------
- Navigation: header links should scroll smoothly to the target sections.
- Responsive layout: verify pages at desktop and mobile widths (use browser dev tools to emulate mobile).
- Forms: any contact/membership forms should validate client-side (they may use `novalidate` and JS validation).
- Interactive JS: check each `*.js` associated with a page for features like toggles, item filters, calculators, or light/dark themes.

How to test functionality (simple checklist)
-------------------------------------------
1. Navigation links: click each nav link and confirm smooth scroll/navigation.
2. Forms: try submitting with invalid values (empty, wrong email) to confirm validation triggers.
3. Responsive: resize the browser or use Chrome DevTools > Toggle device toolbar to test mobile layout.
4. JavaScript interactivity: for any page with a button (e.g., calculate BMI, toggle theme), click and confirm expected behavior.

Preparing screenshots and PDF for submission
-------------------------------------------
1. Take screenshots of each page and important UI states (desktop + mobile). On Windows use Snipping Tool or Print > Save as PDF.
2. Include code snippets (HTML/CSS/JS) and the screenshots in a document (Word or Google Docs).
3. Export or Print to PDF and submit.

Customizing the site
--------------------
- To change text content, edit the corresponding HTML file.
- To change styles, edit `*.css` files (for example`style.css` if present). Try to keep color variables organized at the top.
- To change behavior, edit the page's matching JS file and test in the browser.

Server-side notes (only if you use PHP/MySQL)
--------------------------------------------
- If a page uses PHP endpoints, you'll need XAMPP or another LAMP/WAMP stack:
  - Copy the project folder into `C:\xampp\htdocs\` (or your server document root).
  - Start Apache (and MySQL if you use a database) and open the site via `http://localhost/YourFolder/YourPage.html`.
- Update PHP database credentials inside the PHP files as necessary.

Accessibility & performance tips
--------------------------------
- Add alt attributes to images (e.g., `<img alt="Workout demo">`).
- Ensure form controls have associated `<label>` elements.
- Compress images for faster load times (use 100–200 KB for web photos).

Common issues & fixes
---------------------
- Missing images: check the filename and ensure file is in the same folder as the HTML file.
- JS not running: open browser DevTools (F12) and check the Console for errors; ensure the script is referenced with the correct relative path.
- Fetch errors for PHP endpoints: confirm you're serving the page via HTTP (not `file://`) and that Apache/PHP is running.

Next steps I can help with
-------------------------
- Create a single, consolidated `index.html` that links to all sections/pages.
- Add a small Admin page or JSON file to manage content (images, descriptions) instead of editing HTML directly.
- Produce the PDF deliverable for you (I can assemble screenshots and code snippets into a PDF draft).

Contact / Help
--------------
If you want me to convert this into `README.md` at the project root, or to make the PDF/screenshots for submission, tell me which pages and screenshots you'd like included and I will prepare them.

Good luck — tell me which improvements or deliverables you'd like next.

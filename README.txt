HTML Pocket — iPhone HTML App Launcher

WHAT IT DOES
- Opens the included Pip's Baccarat app immediately.
- Lets you import any future self-contained .html file.
- Remembers the selected HTML on the iPhone.
- Works offline after installation.
- Uses the native iPhone Files picker, not the Documents app.

IMPORTANT
The HTML Pocket folder must be hosted once over HTTPS before iPhone can add it as a Home Screen web app.

GITHUB PAGES SETUP
1. Create a GitHub repository, for example: html-pocket
2. Upload every file and folder from this ZIP to the repository root.
3. Open Settings > Pages.
4. Select Deploy from a branch > main > /(root).
5. Open the published github.io address in Safari on iPhone.
6. Tap Share > Add to Home Screen > Open as Web App > Add.

USING FUTURE HTML FILES
1. Save the .html file to the iPhone Files app.
2. Open HTML Pocket.
3. Tap the three-dot button.
4. Tap Import HTML and choose the file.
5. HTML Pocket remembers it automatically.

Only import self-contained HTML files you trust.


IPHONE VIEWPORT FIX
This build fixes a blue strip / cut-off area at the bottom of the installed Home Screen app.

To update an existing installation:
1. Replace the files in the same GitHub Pages repository with this build.
2. Wait for GitHub Pages to finish deploying.
3. Open HTML Pocket once while online.
4. Fully close it from the iPhone app switcher.
5. Open it again from the Home Screen.

The service-worker cache version has been changed so the new shell replaces the old one.

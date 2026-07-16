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


FULL-SCREEN COVER FIX V3
This version no longer uses the reduced iPhone visual viewport as the app height.
In Home Screen mode, it uses the full screen height and extends the iframe slightly
past the bottom edge so the HTML Pocket blue shell cannot show through.

UPDATE STEPS
1. Replace every file in the existing GitHub Pages repository with this ZIP's files.
2. Wait for GitHub Pages to finish publishing.
3. Open the published site once in Safari.
4. Open HTML Pocket from the Home Screen.
5. Fully close HTML Pocket from the app switcher and reopen it.

If the old version remains cached, remove the Home Screen icon and add it again
from the newly published Safari page.


NO-IFRAME IPHONE FIX
The exact uploaded project still used an iframe to display imported HTML.
iPhone Home Screen mode can reserve the bottom safe area outside an iframe,
which caused the solid blue strip.

This build removes the iframe completely:
- imported HTML becomes the real top-level page
- the three-dot HTML Pocket menu is injected into that page
- the same IndexedDB data is reused, so the currently selected app is preserved
- localStorage in imported apps continues to use the same website origin
- offline support and the Home Screen icon remain

UPDATE
1. Replace the repository files with this build.
2. Wait for GitHub Pages deployment.
3. Open the website once in Safari while online.
4. Fully close HTML Pocket and reopen it.
5. If iOS keeps the old shell, remove the Home Screen icon and add it again.

Preview the single-page site locally (serving via HTTP is recommended so the custom OTF font loads correctly).

PowerShell (Windows) – one command to serve from project root:

1) Open PowerShell in the project folder `d:\Project\GalTech`
2) Run:

```powershell
# starts a static server on port 8000
python -m http.server 8000
```

Then open http://localhost:8000 in your browser.

Alternate: use the included `dev-server.ps1` script which will find Python and start the server.

Notes:
- If images don't appear, ensure the filenames with spaces are not renamed; the HTML uses URL-encoded spaces (e.g., `Group%20831.webp`).
- If the Field Gothic font doesn't load when opening the file using `file://`, run the local server as above.

This folder is filled in automatically -- you normally don't touch it by hand.

To add photos to the gallery:
  1. Put them in your Google Drive folder:  My Drive\New Peru photos
     (subfolders become albums -- e.g. "New Peru photos\2025" adds a 2025 filter)
  2. Run this once from the project folder:
       powershell -ExecutionPolicy Bypass -File .\_import-photos.ps1
  3. Open gallery.html.

The script converts HEIC to JPEG, fixes sideways photos, shrinks them for the
web, and rewrites photos.js -- the list the gallery page reads.

Deleting works the same way: remove a photo from the Drive folder, re-run the
script, and it disappears from the site too. This folder always mirrors Drive.

To caption a photo, type it between the quotes in photos.js. Captions survive
future imports.

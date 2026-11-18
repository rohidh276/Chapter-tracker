CHAPTER TRACKER PWA
===================

Files:
- index.html: your Chapter Tracker app
- manifest.json: installable app metadata
- service-worker.js: offline app-shell caching
- icons/: Android PWA icons (192px and 512px)

INSTALLATION ON ANDROID TABLET
1. Extract this ZIP.
2. Upload the contents of the ChapterTracker folder to a static HTTPS host.
   Keep the folder structure exactly as it is.
3. Open the hosted index.html URL in Chrome on your tablet.
4. Wait for the page to finish loading, then open Chrome's three-dot menu.
5. Choose "Install app" or "Add to Home screen", then confirm.
6. Launch Chapter Tracker from the new home-screen icon.

IMPORTANT
- A PWA and service worker require HTTPS (localhost is the development exception).
- Do not open index.html directly as a file:// page to install it.
- Chapter data is saved in this browser's localStorage on this device.
- Clearing Chrome site data or uninstalling/clearing browser storage may erase saved chapters.
- Offline support starts working after the app shell has been successfully cached once online.
- If you update the app later, change CACHE_NAME in service-worker.js (for example v2) so the new files are cached.

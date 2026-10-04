VOICE ORB — talk to an AI out loud, on your phone or computer, with no API key

WHAT'S IN THIS FOLDER
  index.html               the app
  manifest.webmanifest     makes it installable
  sw.js                    lets it open offline
  icon-*.png               app icons

PUT IT ONLINE (needed for phones: the mic and "Install" only work on https)
  Easiest, free, 1 minute:
  1. Go to https://app.netlify.com/drop
  2. Drag this whole folder onto the page.
  3. Open the link it gives you on your phone.
  (GitHub Pages, Vercel or Cloudflare Pages work the same way.)

TRY IT ON YOUR COMPUTER FIRST
  In this folder run:   python -m http.server 8000
  Then open:            http://localhost:8000

INSTALL ON YOUR PHONE
  Android (Chrome): an "Install Voice Orb" popup appears. Tap Install.
  iPhone (Safari):  the popup shows how: Share → Add to Home Screen.

FIRST RUN
  The AI model downloads once (use Wi-Fi). Phone model ≈ 400 MB.
  After that it runs fully on your device and works offline.
  You can start the download from Settings → "Download model now".

WHICH PHONES CAN RUN THE AI ON-DEVICE
  Android: recent Chrome on most phones from the last ~3 years.
  iPhone:  iOS 26 or newer (Safari).
  Older phones: choose "Google Gemini" in Settings and paste a free key
  from aistudio.google.com. Everything else works the same.

FULLY OFFLINE
  While online, open Settings and tap "Download for offline use".
  That downloads the AI brain and on-device voice recognition (Whisper).
  After that, everything works in flight mode.
  Voice recognition setting:
    Auto      built-in recognition when online, on-device when offline (default)
    On-device always offline, private, works in any language Whisper knows
    Built-in  your phone's recognition (fastest, may need internet)

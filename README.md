# CrossFire PH — Safe Clone (Demo)

Files included:
- index.html
- style.css
- scripts.js
- README.md

Important notes:
- I removed any code that attempted to capture IP, webcam images, geolocation and send them to Telegram (or other third parties).
- The current JS (scripts.js) only provides safe UI demos and local geolocation display (only if the user gives permission).
- If you need consent-based uploads (e.g., user explicitly uploads a screenshot or shares location to your server), I can add:
  - a Flask (or Node) server endpoint with authentication,
  - secure storage + retention policy,
  - client-side consent modal and authenticated POST flow,
  - and admin UI to manage/delete uploaded data.

How to use:
1. Save the 4 files into a folder (e.g., `cf_clone/`).
2. Preview locally: open `index.html` in your browser.
3. To serve over local HTTP: `python -m http.server 8000` and open http://localhost:8000

Ethics & legality:
- Do not add any hidden telemetry or secret tokens that expose users' private data.
- Always obtain explicit, informed consent before collecting camera, location, or other sensitive data.

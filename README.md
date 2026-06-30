# Meri Kashti — Netlify Deployment Package

## Files
- index.html              ← Main platform
- netlify.toml             ← Security headers + redirect config
- netlify/functions/chat.js ← AI proxy function (needs ANTHROPIC_API_KEY)

## Deploy Steps (GitHub Method — Recommended)
1. Create a GitHub repo (e.g. meri-kashti-platform)
2. Upload ALL files using "Add file" → "Upload files" — make sure the
   folder structure is preserved: netlify/functions/chat.js must stay
   inside the netlify/functions folder, NOT in the root.
3. Connect the repo in Netlify: app.netlify.com/start → choose GitHub → select repo
4. In Netlify → Project configuration → Environment variables:
   Add ANTHROPIC_API_KEY = your key from console.anthropic.com
5. Deploy. Check Functions tab — "chat" should be listed.

## Deploy Steps (Drag & Drop Method)
1. Extract this ZIP fully
2. Drag the ENTIRE extracted folder (not just index.html) onto
   Netlify's Deploys page drop zone
3. Set ANTHROPIC_API_KEY in Environment variables
4. Trigger a redeploy after adding the env var

## OTP Demo Mode
Use 123456 as the OTP during registration testing.

© 2025 Meri Kashti · MeriKashti.ai · Chova Lal Suhagpure, Nagpur, India

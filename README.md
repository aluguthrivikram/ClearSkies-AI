# ClearSkies — Clean-air companion

A responsive GenAI-powered assistant prototype for families and communities navigating winter smog and urban air pollution.

## Features
- Personalised daily plan using location, user-entered AQI, household type, home type and commute mode.
- Practical indoor-air, exposure-reduction and low-emission routine suggestions.
- Impact explanations focused on exposure, indoor particle sources and vehicle kilometres.
- Optional Gemini 2.5 Flash integration for conversational, contextual advice.
- Built-in guidance works without an API key.
- Responsive mobile-friendly interface; no framework or build step.

## Run locally
Open `index.html` in a modern browser.

## Enable Gemini
1. Create a Gemini API key in Google AI Studio.
2. Open the app and paste the key into the optional field.
3. Ask a question in the ClearSkies AI section.

**Security note:** This prototype calls Gemini directly from the browser. A key entered here is used only in the current page session and is not saved by this app, but browser-side keys can be exposed through developer tools/network inspection. For production, move Gemini calls to a server-side function, store the key in environment variables, and add rate limiting. Do not commit API keys to GitHub.

## Deploy
- GitHub Pages: create a public repository, upload `index.html` and `README.md`, then enable Pages from Settings → Pages → Deploy from branch → `main` → `/ (root)`.
- Or deploy the folder using Netlify/Vercel static hosting.

## Important limitations
- AQI is entered by the user; no live AQI feed is connected.
- CO₂e avoidance is a clearly labelled illustrative estimate, not a measured result.
- Health guidance is general and not a diagnosis. Users should follow official local AQI guidance and seek medical care for symptoms.
- HEPA filtration advice is general; the app discourages ozone-generating air cleaners.

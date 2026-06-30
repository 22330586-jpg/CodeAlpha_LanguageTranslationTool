# CodeAlpha_LanguageTranslationTool
# CodeAlpha_LanguageTranslationTool

**Lingua** — a language translation tool built for the CodeAlpha AI Internship (Task 1).

A single-file web app. Open `index.html` in any browser — no install, no build, no backend.

## Features
- Enter text and choose **source** and **target** languages (25 languages).
- Translates via the **MyMemory Translation API** (free, no API key).
- Displays the translated text clearly.
- **Swap languages** with one click (also swaps the translated text back).
- **Copy** button and **text-to-speech** (read aloud) for both panels.
- Live character counter, loading and error states.
- Responsive (desktop → mobile), dark UI, keyboard shortcut `Ctrl/Cmd + Enter` to translate.

## How it works
1. The user types text and selects two languages.
2. The app sends the text to the MyMemory API endpoint:
   `https://api.mymemory.translated.net/get?q=TEXT&langpair=SOURCE|TARGET`
3. The JSON response's `translatedText` is shown on screen.
4. Optional features (copy / speech) use the Clipboard API and the Web Speech API.

## Run it
- Locally: double-click `index.html`.
- Deploy: drag the folder onto [Netlify Drop](https://app.netlify.com/drop) or push to GitHub Pages.

## Notes
- The free MyMemory tier allows ~5,000 words/day per anonymous user — fine for a demo.
- No keys are stored in the code, so it's safe to make the repo public.

Built by **[your name]** · CodeAlpha Internship.

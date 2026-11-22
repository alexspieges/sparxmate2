SPARXMATE SCIENCE WEBSITE
=========================

This is a local website you run on your Windows PC. It opens in Chrome.

FEATURES
- Responsive website layout for PC and mobile.
- Biology, Chemistry, Physics and mixed science modes.
- GCSE Year 9, 10 and 11 levels.
- AI explanations and suggested answers.
- Upload a screenshot (PNG, JPG or WEBP) for AI vision.
- Optional Microsoft Edge or Chrome tab sharing: explicitly share the Sparx tab, then capture its current visible frame without manually taking screenshots.
- 30-minute study timer and basic session progress.
- Copy suggested answer.

IMPORTANT
- This website does not log into Sparx or submit homework. Tab reading uses Chrome's explicit screen-share permission and captures only a frame when you press the button.
- You can open Sparx in another tab and explicitly share that tab, or paste a question/upload an image.
- Do not put your Sparx password into SparxMate.
- An OpenAI API key is required. API usage may cost money separately from a ChatGPT subscription.
- Keep your API key private in the local .env file.

SETUP ON WINDOWS
1. Install Node.js LTS from https://nodejs.org/
2. Extract the SparxMate-Website folder somewhere easy to find.
3. In the folder, copy ".env.example" and rename the copy to ".env".
4. Open .env in Notepad and replace put_your_api_key_here with your OpenAI API key.
5. Open Command Prompt in this folder.
6. Run: npm install
7. Run: npm start
8. Keep the Command Prompt window open.
9. In Chrome, visit: http://localhost:3210

USAGE
1. Open Sparx Science in another Chrome tab and sign in there yourself.
2. Return to SparxMate at http://localhost:3210.
3. Click "Connect to Sparx tab". In Chrome's share picker, choose the Sparx Science tab and confirm sharing.
4. Switch back to SparxMate and click "Read current question". This captures the currently visible tab frame for AI vision; it does not continuously monitor the tab.
5. Click "Explain with AI". Review the explanation and copy the suggested answer if useful.
6. When you move to another Sparx question, capture the new current view and ask again.
7. Click "Stop" when finished sharing. Submit your own work on Sparx.

TROUBLESHOOTING
- Website won't open: make sure npm start is still running.
- AI not configured: check .env and restart npm start.
- API error: check the API key, billing/usage limits, and OPENAI_MODEL setting.
- Screenshot too large: use an image smaller than 8 MB.

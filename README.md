# SYNQ AI
**Your work, connected. Your time, reclaimed.**

SYNQ AI is a polished workplace productivity assistant prototype with five connected modules:
- **Smart Compose** — context-aware professional email drafts and tone variations.
- **Meeting Intelligence** — summaries, decisions, action items, owners, and deadlines.
- **Priority Pilot** — task list, priorities, progress, and a suggested daily rhythm.
- **Insight Lab** — concise topic overviews and practical recommendations.
- **SYNQ Copilot** — a conversational entry point to the other tools.

The interface is responsive and uses CSS-only visual design; no image assets are required. This starter runs in **demo mode** with local sample logic, so it does not call a live AI model, send emails, or connect to a calendar. This is intentional: it can be demonstrated without API keys, and it is safe to publish as a starter repository.

## Upload to GitHub without VS Code
1. Download and extract `SYNQ-AI-GitHub-Ready.zip` on your computer.
2. Go to https://github.com and create a repository called `synq-ai`.
3. Open the empty repository and select **Add file → Upload files**.
4. Upload the *contents* of the extracted folder (not the ZIP itself).
5. Commit the files. That's it — you can manage the repository in your browser.

## Run it locally (optional)
You do not need VS Code, but local running requires Node.js:
1. Install Node.js LTS from https://nodejs.org/.
2. Open Terminal or PowerShell in the extracted project folder.
3. Run `npm install`, then `npm run dev`.
4. Open the local address printed by Vite (usually `http://localhost:5173`).

## Deploy it online
After uploading to GitHub, import the repository at https://vercel.com. Vercel should detect Vite automatically. Build command: `npm run build`; output directory: `dist`.

## Connect a real AI model later
Add a server-side endpoint or serverless function that calls your chosen provider. Store API credentials in your hosting platform's environment variables. **Never put private API keys in frontend React code or commit secrets to GitHub.** Validate outputs, handle rate limits, and require human review before external actions.

## Responsible AI
- Treat generated content as a draft, not verified fact.
- Missing task owners or deadlines should be confirmed, not guessed.
- No external actions (sending or scheduling) happen automatically.
- Use synthetic data for demos and do not submit confidential business content to unapproved services.
- Research summaries are illustrative and are not source-verified unless trusted source material is provided and checked.

## Project structure
```text
synq-ai/
├── index.html
├── package.json
├── vite.config.js
├── .env.example
├── README.md
└── src/
    ├── main.jsx
    ├── App.jsx
    └── styles.css
```

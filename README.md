# Meeting Notes AI · Minutia

**Turn meetings into decisions, owners, and next moves.**

[Live Demo](https://keyars.github.io/meeting-notes-ai/) · [Source Code](https://github.com/keyars/meeting-notes-ai)

Minutia is a browser-first meeting notes workspace that transforms messy notes and transcripts into a structured meeting brief: executive summary, decisions, action items, owners, deadlines, risks, and follow-ups.

## Why Minutia

Most meeting-note tools produce a wall of text. Minutia is designed around the work that happens after the meeting. It makes the signal visible, assigns context to actions, and gives teams a concise brief that can be copied or exported.

## Features

- Paste transcripts, notes, or rough bullets
- Structured executive summary
- Decision extraction
- Action-item board with owner, due date, and priority
- Risks and open questions
- Follow-up list
- Source word count and brief-readiness indicator
- One-click summary copy
- Text brief export
- Responsive mobile/desktop experience
- No backend or account required for the demo

## AI integration

The demo uses a deterministic local structuring flow so the project stays runnable without credentials. For production, replace the local generation implementation with a secure server-side LLM endpoint and return the same structured fields used by the UI.

Recommended production response fields: summary, decisions, actions, risks, and followups.

Never put a private model-provider API key in browser code.

## SEO / AEO / GEO strategy

This project uses people-first, crawlable content instead of keyword stuffing. The HTML shell includes a descriptive title, meta description, canonical URL, Open Graph metadata, and SoftwareApplication structured data.

### What is Meeting Notes AI?

Meeting Notes AI is software that turns meeting transcripts or notes into a concise, structured brief containing decisions, action items, owners, risks, and follow-ups.

### What should meeting notes include?

A useful meeting record should make the main outcome easy to scan, then clearly identify decisions, action items, owners, deadlines, unresolved risks, and follow-up work.

### How do you summarize a meeting transcript?

Start with the purpose and outcome, remove repetition, separate confirmed decisions from discussion, convert commitments into action items, and preserve ownership and deadlines.

### Can Meeting Notes AI work without an account?

The Minutia demo runs in the browser and does not require an account or backend.

### Is AI meeting summarization private?

For this demo, meeting content stays in the browser. A production deployment should use server-side model calls, explicit retention controls, and a clear privacy policy.

## Discoverability notes

Search engines and generative search systems benefit from useful people-first content, crawlable pages, strong metadata, and structured information. Google has published current guidance on optimizing for generative search features and structured data; there is no guaranteed shortcut to inclusion in AI answers.

## Local development

npm install
npm run dev
npm run test
npm run build

## Deployment

GitHub Actions verifies tests and the production build, then publishes the Vite output to GitHub Pages.

Live: https://keyars.github.io/meeting-notes-ai/

## Tech stack

React · TypeScript · Vite · Vitest · React Testing Library · Lucide

## License

MIT

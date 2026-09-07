# WBAIT — World Best AI Teacher

An interactive AI-powered learning platform that adapts to how you learn. Single-page app with STEM tutoring, document learning, and offline support.

## Capabilities

- **AI tutoring** — conversation with top-tier LLMs (Anthropic Claude, Google Gemini, and OpenAI-compatible) that adapts explanations to your level
- **STEM engine** — renders math, plots, and diagrams live (KaTeX, math.js, D3)
- **Learn from documents** — upload PDFs, parse and OCR them (pdf.js + Tesseract.js), then study them with AI
- **AI image generation** — visual explanations on demand
- **Offline-first** — service worker caching, lessons work without a connection
- **Accounts** — Supabase auth + storage for progress and saved lessons

## Stack

Claude API · Gemini API · Supabase · Tesseract OCR · pdf.js · D3 · KaTeX · math.js · vanilla JS

## Run

Deploys as a static front-end (Netlify/GitHub Pages compatible). API keys are supplied by the user in-app (saved to `localStorage`) — bring-your-own-key model, so no backend secrets live in this repo.

## Notes

- Tools: OpenAI-style open API for manual mode; one-click reset between sessions
- `sw.js` enables offline caching when present
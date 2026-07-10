# Experts-bureau website

A single-file static site (`index.html` — no build step, no dependencies) for Experts-bureau, a recruitment market intelligence and B2B lead data company.

## Deploy to Vercel

**Option A — Vercel CLI (fastest)**
```bash
npm i -g vercel
cd experts-bureau
vercel
```
Follow the prompts (link/create a project, accept defaults). Vercel auto-detects this as a static site — no framework, no build command needed.

**Option B — GitHub + Vercel dashboard**
1. Push this folder to a new GitHub repo.
2. Go to vercel.com → **Add New Project** → import the repo.
3. Leave all build settings blank/default and click **Deploy**.

**Option C — Drag and drop**
Go to vercel.com/new, drag the `experts-bureau` folder onto the page.

## Before you go live

- Replace `hello@experts-bureau.com` (in the Contact section and footer) with your real inbox — it's used both as a mailto link and as the [FormSubmit](https://formsubmit.co) endpoint that powers the "Request a sample list" form. FormSubmit sends you an email the first time it's used at a new address, asking you to confirm — click that link once and the form goes live.
- Swap in a real logo if you have one; currently it's a styled text wordmark.
- Update the industries/chips list if your actual coverage differs.

## Structure

- `index.html` — everything: markup, CSS (in `<style>`), and a small vanilla JS block for scroll-reveal animation. No external JS libraries.
- Fonts load from Google Fonts (Fraunces, Inter, IBM Plex Mono) via CDN link tags.

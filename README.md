# Ama Events Co. — Booking Site

Front-end for a client project: an event planning and rental business
based in Port Harcourt, Nigeria. This site is the customer-facing intake
layer for an n8n-powered lead triage automation — form submissions here
feed into a workflow that classifies leads, routes replies across
WhatsApp/Instagram/Facebook, logs to Airtable, and notifies the business
owner.

**Live site:** https://ama-events-co-site.vercel.app

## What this covers
- Static site (HTML/CSS/vanilla JS), deployed on Vercel via GitHub
- Two intake flows: full event booking, standalone rental requests
- Forms POST JSON to n8n webhook endpoints
- `CONFIG.DEMO_MODE` flag lets the site run fully functional for demos
  without a live backend attached

## Stack
- Vanilla HTML/CSS/JS — no framework, no build step
- n8n (self-hosted) for backend automation — see [workflow repo/link if you make one]
- Vercel for hosting

## Status
🚧 In progress — webhook endpoints point to a placeholder host until the
n8n instance is publicly reachable.

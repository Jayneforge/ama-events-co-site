# Ama Events Co. — Booking Site

Front-end for a real-world-style client project: an event planning, decor, and rental business based in Port Harcourt, Nigeria. This site is the customer-facing intake layer for an AI-powered n8n automation — form submissions here feed a workflow that triages leads, replies across WhatsApp/Instagram/Facebook, logs to Airtable, and alerts the business owner in real time.

**Live site:** https://ama-events-co-site.vercel.app

## What this covers

- Static site (HTML/CSS/vanilla JS), deployed on Vercel via GitHub
- Two intake flows: full event booking, standalone rental requests
- Forms POST JSON to n8n webhook endpoints
- `CONFIG.DEMO_MODE` flag lets the site run fully functional for demos without a live backend attached

## The automation behind it

This site is one half of the project. The other half is a 41-node n8n workflow that receives these submissions (and inbound WhatsApp/Instagram/Facebook messages), runs them through AI triage, and handles the full lead lifecycle — including real bugs found and fixed during testing, not just a happy-path demo.

**→ [Read the full automation case study](./WORKFLOW.md)**

## Stack

Vanilla HTML/CSS/JS — no framework, no build step · n8n (self-hosted) for backend automation · Vercel for hosting

## Status

Site is fully deployed and connected to a live (dev-tunneled) n8n instance. Automation logic is tested end-to-end; see the [workflow case study](./WORKFLOW.md) for current known limitations before real production use.

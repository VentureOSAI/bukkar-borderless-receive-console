# Bukkar Borderless Receive Console

**Bukkar Ltd — Free Live Tool**
Live URL: https://tools.bukkar.com/borderless-receive-console

## Approval Gate
- **Audience:** African freelancers, creators & developers receiving from international clients
- **Pain class:** B. Borderless-Access Pain
- **Market Gap:**
  - X (audience needs): receive international client payments without sharing bank details, IBAN, or routing numbers — and without the transfer being rejected due to corridor incompatibility
  - Y (market provides): SWIFT bank transfers requiring recipient account details in formats many African banks don't issue in internationally-compatible forms; payment apps requiring both parties on the same platform
  - Z (missing capability): a live, generated, identifier-free receive endpoint shareable with any international client, regardless of the client's bank or the recipient's location
  - Bukkar delivers Z through: Bukkar Instant Payments Gateway — payment links, QR codes, and multi-currency wallet settlement requiring no account details from either party
- **Action enabled:** Receive
- **Pillar:** Borderless Access
- **Monetisation:** Free Personal Access (current status — all tools free until further notice)

## What the tool produces (live, not diagnostic)
1. A generated Bukkar receive link (pay.bukkar.com/r/[slug]-[uid])
2. A live-rendered scannable QR code (via qrcodejs CDN)
3. A downloadable "How to Pay Me" instruction card (Bukkar-branded HTML file)
4. A copyable plain-text payment instruction block for email/WhatsApp

## Deployment
- **GitHub Repo:** bukkar-borderless-receive-console
- **Netlify Project:** bukkar-borderless-receive-console
- **Live URL:** https://tools.bukkar.com/borderless-receive-console

## Deploy Steps
1. Create GitHub repo `bukkar-borderless-receive-console` under BukkarLtd organisation
2. Push all files to repo root
3. In Netlify Pro (VentureOSAI account): New site → Connect to GitHub → publish directory `.` → deploy
4. Rename Netlify project to `bukkar-borderless-receive-console`
5. In `ventureosai-runway` repo, add to `_redirects`:
   `/bukkar/borderless-receive-console/* https://bukkar-borderless-receive-console.netlify.app/:splat 200!`
6. Trigger redeploy of `ventureosai-runway`
7. Verify live: https://tools.bukkar.com/borderless-receive-console

## Files
- `index.html` — complete self-contained live console
- `bukkar-logo.png` — Bukkar brand logo
- `netlify.toml` — deploy config with security headers
- `README.md` — this file
- `.gitignore` — standard ignores
- `POST.txt` — LinkedIn post body + first comment

---
Powered by VentureOS AI · Built by Sceamdo · ventureosai.com
Mohammad Bukkar | Economic Systems Architect and Founder — Sceamdo · VentureOS AI · Bukkar Ltd

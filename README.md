# Edwin Mensah Plange (Jay)

**Solo technical founder. Building tools that solve real problems.**  
Based in Accra, Ghana → relocating to Hamburg, Germany (June 2026)

---

## 🔧 What I'm Building

### [DualProfile](https://chromewebstore.google.com/detail/dualprofile/mdlhdncmaeepcejdbpnjpjlmagmmpkpc) — Live on the Chrome Web Store
> *Show different profile photos to different contacts on WhatsApp Web.*

A production Chrome extension (Manifest V3) I built solo from scratch — architected, shipped, and iterated on with real paying users. The core mechanic: when User A opens a chat with User B, a real-time Convex query determines which photo User A has assigned to User B, and injects it into the WhatsApp Web DOM before it renders.

**Tech stack:**
- `React` + `TypeScript` — popup UI and onboarding flow
- `Convex` — real-time backend, serverless functions, and live P2P queries
- `Cloudinary` — photo upload and CDN delivery
- `Lemon Squeezy` — subscription payments (Free / Pro / Founder tiers)
- `Manifest V3` — service worker, content scripts, `chrome.alarms` for reconciliation

**Problems I solved building this:**
- Cross-browser identity collision (Chrome + Edge sharing `extensionId`) → fixed by making `phoneHash` the primary key, with `extensionId` as a fallback
- Post-install drop-off at 88% → redesigned onboarding flow with inline WhatsApp number capture
- DOM race conditions on WhatsApp Web → MutationObserver + 500ms reconciliation loop
- Group photo leaks across contact switches → self-row guard + isolation by `contactPhoneHash`

🔗 [Landing page](https://vivaup.org) · [Chrome Web Store](https://chromewebstore.google.com/detail/dualprofile/mdlhdncmaeepcejdbpnjpjlmagmmpkpc) · [Demo video](https://x.com/JusticePlange/status/1917779218467021129)

---

## 🧰 Stack & Tools

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat&logo=react&logoColor=61DAFB)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![Convex](https://img.shields.io/badge/Convex-EE342F?style=flat&logoColor=white)
![Cloudinary](https://img.shields.io/badge/Cloudinary-3448C5?style=flat&logo=cloudinary&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=nodedotjs&logoColor=white)
![n8n](https://img.shields.io/badge/n8n-EA4B71?style=flat&logo=n8n&logoColor=white)

---

## 📌 Background

- **IT Compliance Associate** — KPMG Ghana (risk, controls, IS audits)
- **NOC Engineer** — Geoquaye Limited (network operations, uptime)
- **Site Access Coordinator** — American Tower Corporation Ghana (process, multi-stakeholder ops)
- **CompTIA Security+** | **Oracle OCI AI Foundations Associate**
- NCC Level 5 Diploma in Business Information Technology (Ofqual-regulated, 600/3049/5)

---

## 📫 Find Me

[![X](https://img.shields.io/badge/@bnyje-000000?style=flat&logo=x&logoColor=white)](https://x.com/bnyje)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/edwinplange)
[![DualProfile](https://img.shields.io/badge/DualProfile-Live-brightgreen?style=flat)](https://vivaup.org)

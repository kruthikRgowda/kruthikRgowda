# Kruthik B R

### React Native & Frontend Engineer · Expo & New Architecture · Mobile Release Engineering

*TypeScript · React Native · Expo / EAS · Realtime Streaming · Native Modules (Kotlin / Swift)*

[Portfolio](PORTFOLIO_URL) · [LinkedIn](LINKEDIN_URL) · [Email](mailto:kruthikbr2@gmail.com) · [LawWorld on Google Play](PLAY_STORE_URL)

---

## What I build

I am a React Native developer who takes mobile products from architecture through to store release. I'm the sole mobile engineer on **LawWorld**, a production AI legal platform with 10,000+ registered advocates on Google Play, where I own authentication, access control, in-app purchases, real-time streaming, and offline behaviour. I'm comfortable working down to the native layer — custom Expo config plugins, TurboModules in Kotlin and Swift, EAS build pipelines, and OTA release management.

---

## Core Stack

- **Languages** — TypeScript · JavaScript (ES6+) · Java · Kotlin · Swift · HTML5
- **Mobile** — React Native (New Architecture, TurboModules) · Expo · EAS Build & EAS Update (OTA) · Expo config plugins · React Navigation · Apple StoreKit / In-App Purchases
- **Realtime & Data** — Server-Sent Events · WebSocket · Socket.IO · REST APIs · Redux · Context API · SQLite · MongoDB
- **Web & Backend** — React.js · Material UI · Node.js · Express.js
- **Tooling & Release** — Git & GitHub · GitHub Actions · Android Studio · Xcode · Play Console · App Store Connect · npm publishing

---

## Engineering Highlights

- **Mobile Architecture & Ownership** — Sole mobile engineer on a ~110-screen production app with 10,000+ registered advocates, owning mobile architecture, release engineering, and Play Store submission end to end alongside a 3-person backend team.
- **Two-Layer Access Control** — Architected role-based permissions resolved against subscription-tier entitlements, designed so a malformed plan response degrades gracefully instead of stripping paying subscribers of purchased features.
- **Resilient Auth Layer** — Eliminated unintended logouts on unstable networks with a centralized authenticated fetch layer that collapses concurrent token refreshes into a single in-flight request, guards against retry loops, and tolerates offline 401s.
- **In-App Purchases** — Hoisted the StoreKit listener to an app-wide provider so auto-renewals, "Ask to Buy" approvals, and post-outage redeliveries are never dropped, backing a 4-tier subscription group and consumable wallet top-ups with server-side receipt verification.
- **Document Sync Engine** — Prevented silent data loss between concurrent web and mobile editors with a snapshot-diffing sync engine using debounced batching and 413-safe chunking, surfacing a visible failure state instead of failing quietly.
- **Token-by-Token AI Streaming** — Replaced React Native's stock fetch (which buffers entire response bodies) with SSE over `expo/fetch` for streaming AI responses; extended the pattern to WebSocket dictation and Socket.IO live transcription.
- **Release Engineering** — Cut hotfix turnaround from a full store review cycle to a same-day push via EAS Update OTA; authored 7 Expo config plugins and maintain 4 EAS build profiles across Android and iOS.
- **Privacy & Compliance** — Implemented a network-layer AI-disclosure consent gate that blocks third-party AI requests before any user content leaves the device, satisfying Apple's App Store disclosure requirements.

---

## Project Spotlight: rn-network-quality

Open-source React Native **New Architecture TurboModule** that exposes live bandwidth and link-quality signals — replacing the binary online/offline flag most React Native apps rely on.

- **Native Bridging:** Wraps Android `NetworkCapabilities` and iOS `NWPathMonitor` behind a codegen'd TypeScript spec, with implementations in Kotlin and Swift.
- **Production-Ready Packaging:** Ships with a runnable example app, GitHub Actions CI, and semantic-versioned npm releases.

## Project Spotlight: Tenet

Rental and tenancy management app for independent landlords · React Native (Expo), TypeScript, Node.js, MongoDB.

- **Offline-First Ledger:** SQLite-backed rent ledger with an outbox sync queue, so entries recorded on-site without signal reconcile on reconnect without double-posting a payment.
- **Multi-Role Codebase:** Single app serving landlord and tenant roles through per-role navigation trees and server-driven entitlement checks.
- **Landlord Tooling:** Multi-property portfolios, tenant onboarding with lease storage, auto-generated rent schedules, UPI collection with reminder nudges, and maintenance-request threads.

---

## Currently exploring

- Deeper React Native New Architecture internals — Fabric, JSI, and custom TurboModule patterns.
- Hardening OTA release strategies with EAS Update channels and rollout gating.
- Offline-first sync patterns and conflict resolution for mobile-first products.

---

## At a glance

```yaml
role: React Native & Frontend Developer
focus: Mobile architecture · Release engineering · Realtime streaming
stack: React Native (Expo) · TypeScript · Kotlin/Swift (native modules) · Node.js · MongoDB
interests: New Architecture · OTA delivery · Offline-first sync · In-app purchases
timezone: IST (UTC+5:30)
contact: kruthikbr2@gmail.com
linkedin: LINKEDIN_URL
portfolio: PORTFOLIO_URL
```

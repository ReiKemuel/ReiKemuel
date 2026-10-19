# Hi, I'm Rei

**Junior iOS developer · Philippines (UTC+8) · open to remote work**

![Swift](https://img.shields.io/badge/Swift-F05138?logo=swift&logoColor=white)
![SwiftUI](https://img.shields.io/badge/SwiftUI-0D96F6?logo=swift&logoColor=white)
![Combine](https://img.shields.io/badge/Combine-5A5A8E)
![AdMob](https://img.shields.io/badge/Google%20AdMob-EA4335?logo=googleads&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?logo=firebase&logoColor=black)
![Claude Code](https://img.shields.io/badge/Claude%20Code-D97757?logo=anthropic&logoColor=white)

I've shipped features on a live App Store product, working inside a senior dev's existing codebase. A lot of the work was studying his patterns, learning fast, and adapting as I went. Most of what I've built so far has been on Ambio — a small distributed team where I contribute to the monetization and lock-screen layers.

## Featured

**[Ambio](https://apps.apple.com/us/app/ambio-sleep-focus-sounds/id6749637478)** — Ambient sound app for sleep, focus, and relaxation. Live on the App Store since May 2026. Built on a small distributed team (lead engineer + marketing partner in Vietnam).

<p align="center">
  <img src="images/ambio-player.png" width="230" alt="Ambio — sound player">
  <img src="images/ambio-mixes.png" width="230" alt="Ambio — mix and match sounds">
  <img src="images/ambio-focus.png" width="230" alt="Ambio — focus timer">
</p>

My layers of the app:

| Layer | What I built |
|---|---|
| **Monetization** | Google AdMob (banner, rewarded, app-open + frequency cap) and a two-tier premium-access manager built on a Combine `Publishers.CombineLatest` pipeline |
| **Lock screen** | NowPlaying + `MPRemoteCommandCenter` controls (play, pause, stop) wired on top of the app's audio playback |
| **Premium UX** | Rewarded-ad flow, unlock-expiry toast, premium sheet with iPad-aware detents, mood/tag filter chip bar |
| **Firebase** | Analytics + Crashlytics init, AdMob adapter-status logging, structured ad-lifecycle event taxonomy |

## Code you can read

| Repo | What's inside |
|---|---|
| **[AdMobKit](https://github.com/ReiKemuel/AdMobKit)** | The AdMob integration pattern from Ambio, sanitized. Banner cache, rewarded flow, app-open with a 120s cooldown, and a typed `AdLifecycleEvent` enum. Swift Package, iOS 17+. |
| **[TwoTierPremiumAccess](https://github.com/ReiKemuel/TwoTierPremiumAccess)** | The Combine pipeline that derives a single `hasPremiumAccess` flag from a rewarded-ad temporary unlock and a subscription source. Honest notes on the rough edges. Foundation + Combine only. |
| **[Morning Manna](https://github.com/ReiKemuel/morning-manna)** | The one that isn't iOS: an AI newsletter engine built with Claude Code. Turns my own church-service notes into a daily devotional email — current subscriber count: me. The engine is public; the personal content never touches git. |

## In progress

**Gauge: Body Recomposition** — a weight-loss coach that treats your body as a noisy signal. You log a weight and one tap for how well you followed the plan, and it smooths the numbers and tells you once a week whether the plan is working. If the data is too thin, it says so and changes nothing. Built in SwiftUI + SwiftData, and it's the first app that's fully mine. The build is uploaded and it's heading into App Store review, so a lot of what I'm learning now is the part after the code: getting people to actually find an app. Ambio taught me that lesson first.

## Stack

| | |
|---|---|
| **iOS** | Swift · SwiftUI · Combine · async/await · Swift Package Manager · MPNowPlayingInfoCenter · MPRemoteCommandCenter |
| **Monetization** | Google AdMob · premium-access state design |
| **Automation** | Claude Code (custom skills, sub-agents, hooks) · MCP servers (Notion, Gmail, Google Calendar, Firecrawl) · Trigger.dev scheduled tasks · Resend email API · Python and TypeScript scripts |
| **Product** | App Store listing and ASO · pricing and positioning · marketing and distribution (learning this one on purpose) |

## Currently

- Getting Gauge ready to launch, and working on Ambio's distribution now that the features are mostly there
- Working through the AI Automation Society challenge — each lesson ends as a reusable Claude Code skill on my machine, and I'm documenting the learning on LinkedIn
- Open to remote iOS junior roles, mentored apprenticeships, or specialized monetization / iOS-platform-API contract work
- Learning depth on Swift Concurrency design, core AVFoundation, and Django REST through code review

## Reach me

- Email: rkscordero@gmail.com
- LinkedIn: [rei-cordero-877835224](https://linkedin.com/in/rei-cordero-877835224)
- Portfolio: [reikemuel.github.io](https://reikemuel.github.io)

---

_BS Computer Science, University of the People (Jan 2026). English (professional), Filipino / Tagalog (native)._

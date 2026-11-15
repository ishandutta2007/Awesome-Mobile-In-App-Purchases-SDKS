<div align="center">

<a href="https://github.com/ishandutta2007/Awesome-Awesome-Awesome"><img src="https://img.shields.io/badge/Awesome-%E2%9C%94-blueviolet?style=flat-square&logo=github" alt="Awesome"/></a><a href="https://discord.gg/jc4xtF58Ve"><img src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Discord" /></a>
<a href="https://github.com/ishandutta2007/Awesome-Awesome-Awesome"><img src="https://awesome.re/badge.svg" alt="Awesome" /></a>
<a href="https://github.com/ishandutta2007/Awesome-Mobile-In-App-Purchases-SDKS/stargazers"><img src="https://img.shields.io/github/stars/ishandutta2007/Awesome-Mobile-In-App-Purchases-SDKS?style=social" alt="GitHub Stars" /></a>
<a href="https://github.com/ishandutta2007/Awesome-Mobile-In-App-Purchases-SDKS/forks"><img src="https://img.shields.io/github/forks/ishandutta2007/Awesome-Mobile-In-App-Purchases-SDKS?style=social" alt="GitHub Forks" /></a>
<a href="https://github.com/ishandutta2007/Awesome-Mobile-In-App-Purchases-SDKS/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-CC0_1.0-blue.svg?style=flat-square" alt="License: CC0 1.0" /></a>
<a href="https://github.com/ishandutta2077"><img alt="GitHub followers" src="https://img.shields.io/github/followers/ishandutta2007?label=Follow" /></a>

<br/><br/>

<a href="https://github.com/ishandutta2007/Awesome-Mobile-In-App-Purchases-SDKS">
  <img src="assets/banner.svg" alt="Awesome Mobile In-App Purchases &amp; SDKs Banner" width="100%" />
</a>

# 📱 Awesome Mobile In-App Purchases & SDKs (IAP) 💳

> 🚀 A curated list of top **Mobile In-App Purchases (IAP)** and **subscription management SDK platforms** — covering SaaS/hosted commercial infrastructure and open-source frameworks for managing subscriptions, digital product entitlements, receipt validation, and paywall A/B testing across iOS, Android, Flutter, React Native, and Web. ✨
> 
> 🌟 **Star this repo if you find it helpful!** 🌟

</div>

Looking for the best mobile subscription billing engine, StoreKit / Google Play Billing wrapper, or no-code paywall builder? This guide benchmarks commercial platforms and open-source tools with transparent pricing tiers, free tier allowances, valuation metrics, and GitHub community popularity. 💡

---

## 📋 Table of Contents 🧭

- [🌐 Sector Overview & Market Dynamics](#-sector-overview--market-dynamics)
- [🟦 SaaS / Hosted Platforms](#-saas--hosted-platforms)
- [🟩 Open-Source Software & SDKs](#-open-source-software--sdks)
- [📊 Comparison at a Glance](#-comparison-at-a-glance)
- [🔍 Key Selection Criteria](#-key-selection-criteria)
- [🌟 Star History](#-star-history)
- [💖 Support & Sponsorship](#-support--sponsorship)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)

---

## 🌐 Sector Overview & Market Dynamics 📈

The global in-app purchase and mobile subscription market is valued at **$160B–$210B** (projected to exceed **$400B+** by the early 2030s at an 11–14% CAGR), driven by recurring subscription monetization across mobile gaming, creator tools, productivity apps, and streaming services. 💰

The market structure exhibits a dual dynamic:
- 🏰 **Operating System / Payment Gateway Level (Highly Concentrated Duopoly):** Apple (App Store / StoreKit) and Google (Google Play Store / Google Play Billing) hold a near-complete duopoly over mobile runtime distribution and platform checkout rails.
- 🧩 **Subscription Infrastructure & Middleware Layer (Consolidating / Moderately Fragmented):** Market leader RevenueCat anchors enterprise and developer adoption, while specialized challengers like Adapty (paywall experimentation), Purchasely (no-code paywall builders), Qonversion (analytics automation), and Apphud (no-backend architectures) compete aggressively alongside emerging self-hosted open-source alternatives.

---

## 🟦 SaaS / Hosted Platforms ☁️

Commercial, cloud-hosted in-app purchase infrastructure, analytics engines, and paywall management suites. Ranked in descending order by company scale, valuation, and venture funding. 🏆

| Platform | 🏢 Company Scale / Valuation / Revenue | 🏷️ Pricing (Starting Tier) | 🎁 Free Tier Limit | 🎯 Core Specialization & Key Features | 📱 Supported Frameworks |
|---|---|---|---|---|---|
| **[RevenueCat](https://www.revenuecat.com/)** | **$500M Valuation** (~$20M ARR, ~$119M Total Funding Raised) 🦄 | 1% of Monthly Tracked Revenue (MTR) on paid volume above free tier | **Free up to $2,500/mo MTR** (full SDK access, returns to free if volume drops) | Cross-platform subscription backend, receipt validation, subscriber status caching, webhooks, and charts | iOS, Android, React Native, Flutter, Cordova, Unity, Web, macOS |
| **[Adapty](https://adapty.io/)** | **$2.5M+ Funding** (~$4.5M–$7M Estimated ARR) 🚀 | 1% of Monthly Tracked Revenue (MTR) on paid volume above free tier | **Free up to $5,000/mo MTR** (unlocked Pro features including paywall builder & A/B testing) | Mobile-first paywall builder, dynamic price localization, paywall A/B testing, and refund protection | iOS, Android, React Native, Flutter, Unity, Kotlin Multiplatform |
| **[Qonversion](https://qonversion.io/)** | **$2.9M Funding** (~$1.7M Estimated ARR) ⚡ | 0.8% of Monthly Tracked Revenue (MTR) on paid volume above free tier | **Free up to $7,000/mo MTR** (complete feature access including experiments & analytics) | In-app purchase backend, subscription retention automation, no-code paywalls, and cross-channel webhooks | iOS, Android, Flutter, React Native, Unity, Cordova, Capacitor |
| **[Purchasely](https://www.purchasely.com/)** | **$2.2M Funding** (Enterprise / Seed-backed) 🎨 | Custom quote-based pricing (custom tiers based on MAUs and subscriber volume upon sales consultation) | **No permanent free tier** (personalized product demo and tailored sandbox evaluation proof-of-concept upon request) | Enterprise no-code paywall visual designer, real-time native UI rendering without app store resubmission, and omni-channel campaigns | iOS, Android, React Native, Flutter, Cordova, Apple TV, Android TV |
| **[Apphud](https://apphud.com/)** | **Bootstrapped / Self-Sustained** (Profitable private entity) 🛠️ | Starts at **0.99% of MTR** (minimum **$49/month** for Pro plan) | **Free up to $10,000/mo MTR** (14-day grace period when exceeding limit before requiring paid upgrade) | Lightweight subscription SDK architecture explicitly designed to operate with no custom backend required, automated push rules, and paywall experiments | iOS, Android, Flutter, React Native, Unity |

---

## 🟩 Open-Source Software & SDKs 🔓

Community-maintained client libraries, StoreKit/Google Play Billing abstractions, receipt validation utilities, and self-hosted subscription backends. Sorted in descending order by GitHub stargazers. ⭐

| Project | ⭐ GitHub Stars | 💻 Language / Tech Stack | 📜 License | 🏗️ Architecture Type | 📝 Description |
|---|---|---|---|---|---|
| **[SwiftyStoreKit](https://github.com/bizz84/SwiftyStoreKit)** | [![Stars](https://img.shields.io/github/stars/bizz84/SwiftyStoreKit?style=social&color=white)](https://github.com/bizz84/SwiftyStoreKit/stargazers) | Swift 🍏 | MIT | Client Library (Apple) | Lightweight, closure-based In-App Purchases Swift framework for iOS, tvOS, and macOS StoreKit. |
| **[react-native-iap](https://github.com/hyochan/react-native-iap)** | [![Stars](https://img.shields.io/github/stars/hyochan/react-native-iap?style=social&color=white)](https://github.com/hyochan/react-native-iap/stargazers) | TypeScript / Java / Obj-C ⚛️ | MIT | Client Library (Cross-platform) | Standard open-source in-app purchase and subscription module for React Native with OpenIAP compliance across App Store, Google Play, and Amazon. |
| **[RMStore](https://github.com/robotmedia/RMStore)** | [![Stars](https://img.shields.io/github/stars/robotmedia/RMStore?style=social&color=white)](https://github.com/robotmedia/RMStore/stargazers) | Objective-C 🍏 | Apache-2.0 | Client Library (Apple) | Established lightweight iOS library for StoreKit in-app purchases with block-based APIs and receipt verification modules. |
| **[cordova-plugin-purchase](https://github.com/j3k0/cordova-plugin-purchase)** | [![Stars](https://img.shields.io/github/stars/j3k0/cordova-plugin-purchase?style=social&color=white)](https://github.com/j3k0/cordova-plugin-purchase/stargazers) | JS / C++ / Swift 🔌 | MIT | Client Library (Hybrid) | Complete in-app purchase plugin for Apache Cordova, Capacitor, and PhoneGap supporting iOS, Android (Google Play), and Windows. |
| **[merchantkit](https://github.com/benjaminmayo/merchantkit)** | [![Stars](https://img.shields.io/github/stars/benjaminmayo/merchantkit?style=social&color=white)](https://github.com/benjaminmayo/merchantkit/stargazers) | Swift 🍏 | MIT | Client Framework (Apple) | A modern, developer-friendly in-app purchase management framework for iOS with built-in subscription state management, product display models, and receipt validation. |
| **[in-app-purchase](https://github.com/voltrue2/in-app-purchase)** | [![Stars](https://img.shields.io/github/stars/voltrue2/in-app-purchase?style=social&color=white)](https://github.com/voltrue2/in-app-purchase/stargazers) | Node.js 🟢 | MIT | Backend Receipt Validator | Server-side receipt validation library for Node.js handling Apple App Store, Google Play, Amazon, Roku, and Windows Store. |
| **[TPInAppReceipt](https://github.com/tikhop/TPInAppReceipt)** | [![Stars](https://img.shields.io/github/stars/tikhop/TPInAppReceipt?style=social&color=white)](https://github.com/tikhop/TPInAppReceipt/stargazers) | Swift 🍏 | MIT | Local Receipt Validator | Pure Swift library for reading and validating Apple In-App Purchase PKCS#7 receipt payloads locally on-device with OpenSSL/ASN.1 parsing. |
| **[store-receipt-validator](https://github.com/aporat/store-receipt-validator)** | [![Stars](https://img.shields.io/github/stars/aporat/store-receipt-validator?style=social&color=white)](https://github.com/aporat/store-receipt-validator/stargazers) | PHP 🐘 | MIT | Backend Receipt Validator | Modern PHP service for validating mobile in-app purchase receipts from Apple App Store, Google Play, and Amazon Appstore. |
| **[Wildberry](https://github.com/ProjWildBerry/wildberry)** | [![Stars](https://img.shields.io/github/stars/ProjWildBerry/wildberry?style=social&color=white)](https://github.com/ProjWildBerry/wildberry/stargazers) | TS / React / PostgreSQL 🍇 | MIT | Self-Hosted Backend | Open-source, all-in-one in-app purchase and subscription management backend server with receipt validation, webhooks, and revenue analytics. |
| **[Cranpose StoreKit](https://github.com/samoylenkodmitry/Cranpose)** | [![Stars](https://img.shields.io/github/stars/samoylenkodmitry/Cranpose?style=social&color=white)](https://github.com/samoylenkodmitry/Cranpose/stargazers) | Rust / Swift 🦀 | Apache-2.0 / MIT | Multi-platform Adapter | StoreKit 2 and Google Play Billing integration module within the Cranpose cross-platform Rust GUI framework. |
| **[BillingHelper](https://github.com/mvojtkovszky/BillingHelper)** | [![Stars](https://img.shields.io/github/stars/mvojtkovszky/BillingHelper?style=social&color=white)](https://github.com/mvojtkovszky/BillingHelper/stargazers) | Kotlin 🤖 | MIT | Client Library (Android) | Streamlined Kotlin helper for Android's Google Play Billing Library simplifying connection lifecycles, query batches, purchase tokens, and signature checks. |
| **[RevenueDot](https://github.com/revenuedot/revenuedot)** | [![Stars](https://img.shields.io/github/stars/revenuedot/revenuedot?style=social&color=white)](https://github.com/revenuedot/revenuedot/stargazers) | TS / Docker / Postgres 🔄 | AGPL-3.0 / MIT | Self-Hosted Backend | Self-hostable, open-source RevenueCat-compatible backend drop-in proxy allowing existing apps using RevenueCat SDKs to switch to their own private infrastructure. |

---

## 📊 Comparison at a Glance ⚖️

| Solution | Deployment | License / Cost | Backend Infrastructure | Receipt Validation | Paywall A/B Testing | Cross-Platform Sync | Primary Use Case |
|---|---|---|---|---|---|---|---|
| **RevenueCat** | Cloud SaaS | Free up to $2.5k MTR, then 1% | Managed Cloud | Server-side (Cloud) | ✅ Yes | ✅ iOS, Android, Web, Desktop | Industry benchmark for mobile subscription ops |
| **Adapty** | Cloud SaaS | Free up to $5k MTR, then 1% | Managed Cloud | Server-side (Cloud) | ✅ Advanced | ✅ iOS, Android, Cross-platform | Paywall experiments, rapid LTV/pricing iteration |
| **Qonversion** | Cloud SaaS | Free up to $7k MTR, then 0.8% | Managed Cloud | Server-side (Cloud) | ✅ Yes | ✅ iOS, Android, Cross-platform | Retention automation & purchase analytics |
| **Purchasely** | Cloud SaaS | Custom Quote | Managed Cloud | Server-side (Cloud) | ✅ No-Code Designer | ✅ Mobile & Connected TV | Enterprise visual paywalls without code releases |
| **Apphud** | Cloud SaaS | Free up to $10k MTR, then 0.99% min $49 | Serverless / Cloud | Server-side (Cloud) | ✅ Yes | ✅ Mobile & Cross-platform | Fast setup with zero custom server requirements |
| **SwiftyStoreKit** | Client Library | MIT (Free) | None (Client-only) | On-device / Apple verifyReceipt | ❌ No | ❌ Apple Ecosystem only | Clean Swift StoreKit implementation |
| **react-native-iap** | Client Library | MIT (Free) | None (Client-only) | Pluggable / Developer backend | ❌ No | ✅ React Native (iOS & Android) | Standard React Native in-app purchase interface |
| **Wildberry** | Self-Hosted | MIT (Free) | Docker + PostgreSQL | Server-side (Self-hosted) | ❌ Roadmap | ✅ iOS & Android | Complete self-hosted private subscription backend |
| **RevenueDot** | Self-Hosted | AGPL-3.0 (Free) | Docker + PostgreSQL | Server-side (Self-hosted) | ✅ Built-in | ✅ RevenueCat SDK compatible | Private drop-in migration from RevenueCat |

---

## 🔍 Key Selection Criteria 🎯

When evaluating in-app purchase and mobile subscription platforms, consider:

1. 🏢 **Self-Hosted vs. Cloud Infrastructure:** Cloud SaaS (RevenueCat, Adapty) handles App Store server notifications (ASSN v2), Google Real-Time Developer Notifications (RTDN), subscription renewal states, and database scaling. Open-source solutions (Wildberry, RevenueDot) give total privacy, data sovereignty, and eliminate revenue-sharing cutoffs at the cost of infrastructure maintenance.
2. 🧪 **Paywall Flexibility & Remote Configuration:** If marketing or growth teams need to iterate on paywalls without native app re-releases, no-code visual paywall editors (Purchasely, Adapty, RevenueCat Paywalls) drastically accelerate iteration speed.
3. 🔄 **Cross-Platform Entitlement Syncing:** If you support mobile and web subscriptions, ensure your engine provides webhooks and REST APIs to sync entitlements across Stripe, Google Play Billing, and Apple StoreKit.
4. 💸 **Volume Pricing Tiers:** Calculate your total Monthly Tracked Revenue (MTR). Free tier limits vary significantly: Apphud ($10K/mo), Qonversion ($7K/mo), Adapty ($5K/mo), and RevenueCat ($2.5K/mo).

---

## 🌟 Star History

[![Star History Chart](https://www.star-history.com/svg?repos=ishandutta2007/Awesome-Mobile-In-App-Purchases-SDKS&type=date&legend=top-left)](https://www.star-history.com/#ishandutta2007/Awesome-Mobile-In-App-Purchases-SDKS&type=date&legend=top-left)

---

## 💖 Support & Sponsorship

Thank you for visiting and supporting this curated resource! ☕

If this project helped you save time, compare monetization SDKs, or architect your mobile in-app purchase infrastructure, please consider supporting continued maintenance:

- ⭐ **Star this repository** to help others discover it.
- 🍴 **Fork and contribute** new SDKs, helpers, or updates.
- 📢 **Share** with fellow mobile developers, indie hackers, and subscription teams.
- ☕ **Buy a coffee or sponsor** ongoing research and maintenance via the [GitHub Sponsor Dashboard](https://github.com/sponsors/ishandutta2007).

---

## 🤝 Contributing 🚀

Contributions are warmly welcomed! To suggest a new open-source repository or SaaS tool:

1. Check that the project is actively maintained.
2. Format the entry according to the corresponding table structure above.
3. Submit a pull request with details on license, tech stack, and primary features.

---

## 📄 License ⚖️

This repository and curated list are released under the [CC0 1.0 Universal (Public Domain)](LICENSE). Individual linked software and SDKs retain their respective open-source or proprietary licenses.

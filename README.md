# Awesome-Mobile-In-App-Purchases-SDKS

# Awesome Mobile In-App Purchases & SDKs

> A curated list of top Mobile In-App Purchases and SDK platforms — both SaaS/Hosted commercial solutions and open-source alternatives for managing subscriptions, paywalls, and purchase infrastructure across iOS and Android.
> 🌟 Star this repo if you find it useful! 🌟

---

## 📋 Table of Contents

- [SaaS / Hosted Platforms](#-saas--hosted-platforms)
  - [RevenueCat](#revenuecat)
  - [Adapty](#adapty)
  - [Qonversion](#qonversion)
  - [Purchasely](#purchasely)
  - [Apphud](#apphud)
- [Open-Source Software](#-open-source-software)
  - [RevenueDot](#revenuedot)
  - [Wildberry](#wildberry)
  - [Google Play Billing Helper (BillingHelper)](#google-play-billing-helper-billinghelper)
  - [StoreKit Adapters (Cranpose, Flutter)](#storekit-adapters-cranpose-flutter)

---

## 🟦 SaaS / Hosted Platforms

Commercial, cloud-hosted Mobile In-App Purchases and SDK platforms. These are not open-source but are included as reference points for feature comparison.

### RevenueCat
**Type:** Cross-platform subscription infrastructure with open-source SDKs
RevenueCat is the most widely adopted commercial subscription backend, providing a unified API for iOS, Android, and web purchases. It handles receipt validation, subscription status tracking, webhooks, and analytics (MRR, churn, conversion) [citation:6]. **Important licensing nuance:** RevenueCat's backend is a hosted service, but its SDKs are open source under the MIT license [citation:10]. Pricing is free up to $2,500 in monthly tracked revenue, then 1% of tracked revenue [citation:10].

### Adapty
**Type:** Subscription management with paywall A/B testing
Adapty provides subscription infrastructure with a focus on paywall optimization, A/B testing, and real-time analytics. It is positioned for mobile-first companies wanting to iterate on pricing and paywall design. Pricing is free under $5K monthly revenue, then 1% of monthly revenue [citation:3]. Adapty has no direct importer to open-source alternatives, requiring manual recreation of products and entitlements during migration [citation:3].

### Qonversion
**Type:** Cross-platform purchase infrastructure with automation
Qonversion provides SDKs for iOS, Android, React Native, Flutter, Cordova, and Capacitor, with a focus on purchase infrastructure, revenue analytics, and engagement automation [citation:4]. Pricing is free up to $7K monthly tracked revenue, then 0.8% of all tracked revenue [citation:12]. Its migration guide uses `syncHistoricalData()` on the client and receipt file handoff on the server [citation:12].

### Purchasely
**Type:** No-code paywall and subscription platform
Purchasely provides a no-code paywall builder alongside subscription infrastructure, allowing teams to design and deploy paywalls without app releases. It is listed as an alternative to Adapty and RevenueCat in comparison directories [citation:5].

### Apphud
**Type:** Lightweight subscription SDK with no backend required
Apphud provides a Flutter SDK (and native SDKs) for managing auto-renewable subscriptions and in-app purchases, explicitly positioned as requiring **no backend** [citation:1]. It includes paywall management (Rules), push notification handling, and session management. Recent versions require `compileSdk 35` or higher on Android (Google Play Billing Library 9) [citation:1]. **Note:** Apphud's SDK is described as open-source in its package description, but the backend service is commercial.

---

## 🟩 Open-Source Software

Self-hosted, community-driven Mobile In-App Purchases and SDK tools. The open-source ecosystem spans **RevenueCat-compatible backends**, **Google Play Billing helpers**, and **StoreKit adapters**.

### RevenueDot
**Stack:** Server (AGPL-3.0) / SDKs (MIT) / TypeScript | **License:** AGPL-3.0 (server) / MIT (SDKs) [citation:10]
RevenueDot is the most notable open-source **RevenueCat alternative**, implementing the API that RevenueCat SDKs call so existing apps can switch backends by setting a proxy URL [citation:10]. Key characteristics:
- **Self-hostable**: runs on Docker and Postgres, with server code on GitHub under AGPL-3.0 [citation:10]
- **SDK compatibility**: forked from RevenueCat's MIT-licensed SDKs, so code imports `RevenueCat` and calls `Purchases` [citation:3]
- **Cloud pricing**: free until apps make $10,000/month, then 0.5% of revenue above that, capped at $999/month [citation:10]
- **Feature set**: paywalls, experiments, targeting, charts, Customer Center, virtual currencies are built; some features still missing versus RevenueCat [citation:10]
- **Migration**: no importer for Adapty or Qonversion; products and entitlements must be recreated manually [citation:3][citation:12]

**Important:** RevenueDot is newer than RevenueCat and still catching up feature-by-feature [citation:10]. The server is AGPL-3.0, meaning if you modify it and offer it as a network service, source obligations apply.
**Best for:** Teams wanting an open-source backend for RevenueCat-compatible SDKs with self-hosting options, accepting a newer project and some feature gaps versus RevenueCat.

### Wildberry
**Stack:** Server (Go?/check) / SDKs (MIT) | **License:** Open Source (framework) [citation:6]
Wildberry is a free, open-source in-app purchase server with cross-platform support, providing a backend and wrapper around StoreKit and Google Play Billing [citation:6]. Key features include:
- **Server-side receipt validation**
- **Webhooks** for purchases, renewals, cancellations
- **Subscription status tracking** across iOS, Android, and web
- **Analytics** (conversion, MRR, churn)
- **Integrations** with analytics and attribution tools
- **Custom backend URL** support for self-hosting [citation:6]

The React Native SDK (`react-native-purchases`) allows configuration with a custom `url` parameter pointing to your own Wildberry server [citation:6]. **Note:** The package is published as `wildberry-purchase` on npm, with documentation at docs.wildberry.com.
**Best for:** Teams wanting a fully open-source purchase backend with self-hosting and cross-platform SDK support, accepting a smaller ecosystem than RevenueDot or RevenueCat.

### Google Play Billing Helper (BillingHelper)
**Stack:** Kotlin | **License:** Open Source (GitHub) [citation:7]
BillingHelper is a Kotlin library that simplifies the use of **Google Play Billing Library (v9.0.0)**, handling client connection, querying product details and owned purchases, different purchase types, acknowledging purchases, and verifying purchase signatures [citation:7]. It is a **client-side helper** rather than a full subscription backend—it does not provide receipt validation, analytics, or cross-platform entitlement management. Other similar helpers include `billy` (Flowable wrapper for Compose) and `billing-suspend` (coroutines wrapper) [citation:7][citation:14].
**Best for:** Android developers wanting to simplify Google Play Billing integration without adopting a full subscription platform, accepting a narrow scope.

### StoreKit Adapters (Cranpose, Flutter)
**Stack:** Swift/Rust (Cranpose) / Dart (Flutter) | **License:** Open Source [citation:8]
Cranpose StoreKit connects Apple's **StoreKit 2** purchase service to the Cranpose framework, reading products and transactions, verifying signed transactions on-device, and publishing store state and purchase events [citation:8]. It requires iOS 15/macOS 12 minimum and active Xcode. For Flutter, community plugins wrap StoreKit and Google Play Billing but typically lack a unified backend for cross-platform entitlement management [citation:7].
**Best for:** Developers using specific frameworks (Cranpose, Flutter) wanting direct StoreKit integration without a subscription platform, accepting framework-specific dependencies.

---

## 📊 Comparison at a Glance

| Software | License | Stack | Self-Hostable Backend | RevenueCat-Compatible | Cross-Platform | Best For |
|----------|---------|-------|----------------------|------------------------|----------------|----------|
| **RevenueCat** | Proprietary (SDKs MIT) | Cloud + SDKs | ❌ | N/A | ✅ | Industry standard |
| **Adapty** | Proprietary | Cloud + SDKs | ❌ | ❌ | ✅ | Paywall A/B testing |
| **Qonversion** | Proprietary | Cloud + SDKs | ❌ | ❌ | ✅ | Purchase automation |
| **Apphud** | Proprietary (SDK open-source) | Cloud + SDKs | ❌ (no backend needed) | ❌ | ✅ (Flutter) | Lightweight no-backend |
| **RevenueDot** | AGPL-3.0 / MIT SDKs | Server + SDKs | ✅ Docker/Postgres | ✅ | ✅ | Open-source RevenueCat alt |
| **Wildberry** | Open Source | Server + SDKs | ✅ Custom URL | ❌ | ✅ (React Native) | Full OSS purchase backend |
| **BillingHelper** | Open Source | Kotlin | ❌ (Client-only) | ❌ | ❌ (Android) | Google Play Billing helper |
| **Cranpose StoreKit** | Open Source | Swift/Rust | ❌ (Client-only) | ❌ | ❌ (Apple) | StoreKit 2 adapter |

---

## 🤝 Contributing

Contributions are welcome! If you know of an open-source Mobile In-App Purchases or SDK tool that should be listed here, please open a pull request with:

- Project name and URL
- Brief description (1–2 sentences)
- Stack and license
- Why it stands out

Please ensure the project is actively maintained (releases within the last 12 months) and genuinely open-source (or clearly note if it is source-available but not OSI-approved, as with RevenueDot's AGPL server).

**Note on the open-source ecosystem:** The in-app purchase space is **dominated by commercial platforms** because receipt validation, cross-platform entitlement management, and analytics require reliable infrastructure. **RevenueCat** leads adoption but is a hosted service—only its SDKs are open source [citation:10]. **RevenueDot** is the most direct open-source alternative, explicitly designed to be RevenueCat-compatible so existing SDK integrations can switch backends with a proxy URL change [citation:10]. **Wildberry** offers a fully open-source purchase backend with self-hosting support [citation:6]. **Apphud** is notable for requiring no backend at all, though its service is commercial [citation:1]. For client-side helpers, **BillingHelper** and **Cranpose StoreKit** simplify native billing integration but do not provide subscription management [citation:7][citation:8]. No open-source project fully replicates RevenueCat's track record and feature completeness, but RevenueDot covers the core workflow for teams wanting an open-source backend.

---

## 📄 License

This list is released under CC0 1.0 Universal (Public Domain). The software projects listed retain their respective licenses.

---

⭐ **If this list helped you discover a useful tool, please star the repo!** ⭐

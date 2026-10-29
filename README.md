# Awesome-Customer-Loyalty-Rewards

## Top Customer Loyalty & Rewards Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Cashback Networks, Points Programs & Self-Hosted Loyalty Engines*  

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Customer Loyalty & Rewards**. These tools enable merchants and platforms to incentivize repeat purchases, reward referrals, and build coalition programs—turning transactional shoppers into habitual customers through cashback, points, and tiered benefits.



**Examples** include Shop Cash, Rakuten Rewards, Ibotta, Drop, Fetch Rewards, Upside, TopCashback, Honey Gold, Lolli, and Swagbucks (the category leaders).



**Open-source emphasis**: Customer Loyalty & Rewards is a domain where open-source tooling is **fragmented but genuinely functional for merchant-side and developer-led programs**. The strongest active projects are **loyalty-card** (a Go REST API for managing guests, scores, and tags with Docker support) , **Premio** (a full-stack loyalty program with cashier/manager roles and QR codes) , and **Points and Rewards for WooCommerce** (a GPL plugin adding points earning and redemption to WooCommerce stores) . For blockchain-native coalition programs, **Tapestry** demonstrates cross-merchant point conversion on Stellar . The critical gap: **no open-source project replicates the consumer-facing cashback networks** of Rakuten, Ibotta, or Fetch—those rely on massive retailer partnerships and affiliate tracking infrastructure that open-source cannot replicate.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-products)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Shop Cash](https://shop.app/)**  

  Shopify's consumer rewards program within the Shop app; users earn Shop Cash on eligible purchases paid with credit/debit cards, redeemable at checkout across participating Shopify merchants; no cash value and non-transferable .



- **[Rakuten Rewards](https://www.rakuten.com/)**  

  Cashback network partnering with 3,500+ stores; users shop through Rakuten's site, app, or browser extension to earn Cash Back, paid quarterly via check or PayPal; supports in-store offers via linked cards and dining cashback .



- **[Ibotta](https://ibotta.com/)**  

  Cashback app for groceries and everyday purchases; users add offers before shopping, then redeem via linked loyalty accounts or receipt uploads; payouts to bank or gift cards at $20 minimum; claims $1.8B+ paid to users .



- **[Drop](https://joindrop.com/)**  

  Card-linked coalition loyalty program; users link credit/debit cards and select up to five partner brands to earn points automatically on purchases; **caution**: reports indicate points may not be redeemable as of 2025 .



- **[Fetch Rewards](https://fetch.com/)**  

  Receipt-scanning rewards app; users snap paper or email receipts to earn points, redeemable for gift cards; also offers in-app shopping and mobile games for additional points .



- **[Upside](https://www.upside.com/)**  

  Cashback app for gas, groceries, and dining; users claim offers before purchase, pay normally, and receive cash back after transaction verification; funded by participating retailers .



- **[TopCashback](https://www.topcashback.com/)**  

  Cashback website passing 100% of retailer commissions back to members; users shop through TopCashback links to earn rebates; supports stacking with cashback credit cards .



- **[Honey Gold](https://www.joinhoney.com/)**  

  PayPal-owned rewards program; users earn Gold on eligible purchases at partner stores, convertible to gift cards; integrated with Honey's coupon-finding browser extension .



- **[Lolli](https://www.lolli.com/)**  

  Bitcoin and cashback rewards app; users earn Bitcoin or cash on purchases and by playing mobile games; positions Bitcoin as a savings vehicle .



- **[Swagbucks](https://www.swagbucks.com/)**  

  Rewards platform earning SB points through shopping, surveys, games, and offers; points redeemable for gift cards or PayPal cash; features gamified "Swago" bingo boards .



## Open-Source GitHub Projects



### Merchant-Side Loyalty Engines



- **[loyalty-card (patricksferraz)](https://github.com/patricksferraz/loyalty-card)**  

  Modern open-source **RESTful loyalty program backend** (Go, Fiber, GORM, GPLv3) . Features guest management (create/retrieve), score management (create, retrieve, use/redeem, tag), and tag search; supports PostgreSQL and SQLite; Docker Compose deployment with Swagger/OpenAPI documentation. **The cleanest developer-oriented foundation for building a custom loyalty API**—but it is a backend service, not a complete program with UI or earning rules.



- **[Premio (abarlow4944)](https://github.com/abarlow4944/Premio)**  

  Full-stack **customer loyalty program application** (React/Vite/Tailwind frontend, Node/Express/Prisma/PostgreSQL backend) . Features three roles (Regular, Cashier, Manager), point accumulation and redemption, transfers between users, event RSVPs with organizer point awards, promotions, unique QR codes per user, password reset/account activation emails, and analytics with Recharts. Deployed on Railway with demo credentials available. **The most complete open-source loyalty application** with a working UI—but it is a standalone program rather than a pluggable module for existing stores.



### E-commerce Plugins



- **[Points and Rewards for WooCommerce (wpswings)](https://github.com/wpswings/points-and-rewards-for-woocommerce)**  

  Open-source **WooCommerce loyalty points plugin** (GPL) . Features points on sign-ups, purchases (fixed or percentage-based), referrals (social sharing to Facebook/Twitter/Email/WhatsApp), and order ranges; redemption on cart or checkout with configurable conversion; gamification (spin-the-wheel, user badges); compatibility with Klaviyo, Smart Coupons, WooCommerce Subscriptions, and MultiVendorX. **The most feature-complete open-source WooCommerce loyalty option**—but it is WooCommerce-specific.



- **[nopCommerce Reward Points](https://github.com/nopsolutions/nopcommerce-docs/blob/c79247d279d56bf21725cf48e9a30083fc165d43/en/running-your-store/promotional-tools/reward-points.md)**  

  Built-in **reward points functionality** within nopCommerce (open-source .NET e-commerce) . Features configurable exchange rate (points to currency), minimum/maximum points per order, points for purchases and registration with validity periods, multi-store accumulation, and checkout redemption. **For .NET stores**—native functionality rather than a third-party plugin.



### Blockchain & Coalition Loyalty



- **[Tapestry (AlAfiz)](https://github.com/AlAfiz/tapestry)**  

  Open-source **coalition loyalty protocol on Stellar Soroban** . Features per-merchant SEP-41 loyalty tokens, cross-merchant redemption at on-chain conversion rates (e.g., Cafe A → Bookshop B at 4:5), rolling issuance caps to prevent abuse, settlement contract with net obligation ledger, and history queries. Live on Stellar Testnet with dashboard. **The most innovative open-source approach to coalition loyalty**—but it is blockchain-native and requires Stellar ecosystem knowledge.



- **[LoyalPyME (R3v180)](https://github.com/R3v180/LoyalPyME)**  

  Open-source **integrated loyalty and hospitality platform** for SMEs (React, Node.js, PostgreSQL) . Features LoyalPyME Core (LCo) for loyalty: tiers, rewards catalog, customer dashboard, point adjustment, and redemption; and LoyalPyME Camarero (LC) for hospitality: digital menu, ordering, Kitchen Display System, and automatic point accrual on payment. Version v1.22.0 with stable loyalty core. **The most comprehensive open-source SME loyalty + ordering platform**—but it is Spanish-language focused and combines two distinct modules.



### Additional Strong Open-Source Options



- **GopherMart (thalq)** — Go loyalty points system with user registration, order management, balance, and withdrawal requests; interacts with an external accrual system . **Minimal reference implementation**—useful as a starting point for the points ledger pattern, not production-ready (tests incomplete).

- **housrCash (V-Stojkovic)** — Cashback rewards concept implementation (Node/MySQL/React) . **Hackathon project**—demonstrates the cashback data model but not production-hardened.

- **GoGoCash Agentic-Commerce-Protocol** — Affiliate cashback platform with Firebase auth, Crossmint Web3 wallets, and multi-chain withdrawals . **Affiliate-network-focused** rather than merchant loyalty.

- **No open-source equivalent to Rakuten or Ibotta exists** — The retailer network, affiliate tracking, and consumer app scale of cashback networks are not replicable by open-source software; they require business development and partnership infrastructure.



**Frameworks for building custom systems**: For a **WooCommerce store**, Points and Rewards provides the most complete plugin . For a **custom loyalty API**, loyalty-card provides a clean Go backend . For a **full-stack standalone program**, Premio offers a working application . For **blockchain coalition loyalty**, Tapestry demonstrates cross-merchant point conversion . No open-source project replicates the consumer cashback network model—those require commercial partnerships.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Loyalty and rewards platforms handling user purchase data must comply with applicable privacy regulations (GDPR, CCPA) and consumer protection laws; cashback and points programs may have regulatory implications (escheatment, tax reporting) depending on jurisdiction.

- **Open-source loyalty & rewards is strongest for merchant-side programs**—WooCommerce plugins and custom backends provide functional point systems . However, **no open-source project replicates the consumer-facing cashback networks** of Rakuten, Ibotta, or Fetch, which depend on retailer partnerships and affiliate tracking infrastructure. Organizations seeking coalition network effects should evaluate commercial platforms.

- Verify license terms for commercial use; loyalty-card uses GPLv3 , Premio is open-source (check repository) , and Points and Rewards is GPL .



---



**Made for merchants, loyalty program managers, and developers building rewards infrastructure.**  

Let's make customer loyalty more open, but with clear eyes about the network-effect moat that consumer cashback platforms hold.

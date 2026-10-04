<p align="center"><!-- awesome:hero --><img src=".github/assets/hero.gif" width="100%" alt="Animated isometric scene: agent bots queue on a path to a checkout terminal, each pays by dropping a coin into its slot, the display flashes a check and a receipt rises, then a box lifts off a storefront shelf and glides onto the agent, who rolls off with it."><!-- /awesome:hero --></p>

<!-- awesome:title --><h1 align="center">Awesome Agentic Commerce</h1><!-- /awesome:title -->

<p align="center"><!-- awesome:tagline -->Protocols, payment rails, storefront integrations and tools that let AI agents discover, buy and pay.<!-- /awesome:tagline --></p>

<!-- awesome:badges -->
<p align="center">
  <a href="https://awesome.re"><img src="https://awesome.re/badge.svg" alt="Awesome"></a>
  <a href="contributing.md"><img src="https://img.shields.io/badge/PRs-welcome-F97316" alt="PRs welcome"></a>
  <a href="https://github.com/ianwieds/awesome-agentic-commerce/commits/main"><img src="https://img.shields.io/github/last-commit/ianwieds/awesome-agentic-commerce?color=F97316" alt="Last commit"></a>
</p>
<!-- /awesome:badges -->

Agentic commerce is AI agents finding products, paying for services and checking out for a person, and businesses selling to them. This list covers the protocols, payment rails, storefront integrations, developer tools and research behind it.

## Contents

- [Protocols and specs](#protocols-and-specs)
- [Payment networks and providers](#payment-networks-and-providers)
- [Agent payment platforms](#agent-payment-platforms)
- [Shopping agents and storefronts](#shopping-agents-and-storefronts)
- [SDKs and tools](#sdks-and-tools)
  - [Commerce protocol tooling](#commerce-protocol-tooling)
  - [x402 and MPP](#x402-and-mpp)
  - [Lightning and L402](#lightning-and-l402)
  - [Agent wallets and toolkits](#agent-wallets-and-toolkits)
- [Discovery and directories](#discovery-and-directories)
- [Benchmarks and research](#benchmarks-and-research)
- [Guides](#guides)
- [Related lists](#related-lists)
- [Contributing](#contributing)

## Protocols and specs

- [A2A x402 Extension](https://github.com/google-agentic-commerce/a2a-x402) - Extension that adds x402 stablecoin payments to Agent2Agent calls between agents.
- [Agent Commerce Kit](https://github.com/agentcommercekit/ack) - Catena Labs patterns and code for agent identity, payments and verifiable receipts.
- [Agent Payments Protocol (AP2)](https://github.com/google-agentic-commerce/AP2) - Google protocol that uses signed mandates to prove a user authorized an agent's purchase.
- [Agentic Commerce Protocol (ACP)](https://github.com/agentic-commerce-protocol/agentic-commerce-protocol) - OpenAI and Stripe spec for agent checkout and delegated payment with merchants.
- [Agentic Services Protocol](https://github.com/ProsusAI/agentic-services-protocol) - Prosus spec for how agents discover, order and track fulfillment of services.
- [ERC-8004 Trustless Agents](https://eips.ethereum.org/EIPS/eip-8004) - Ethereum standard for onchain agent identity, reputation and validation registries.
- [ERC-8183 Agentic Commerce](https://eips.ethereum.org/EIPS/eip-8183) - Ethereum standard for jobs between agents with an escrowed budget and attested delivery.
- [KYAPay](https://github.com/skyfire-xyz/kyapay) - Skyfire protocol that carries agent identity and payment together in signed JWTs.
- [L402](https://github.com/lightninglabs/L402) - Lightning Labs spec that pays for HTTP APIs over Lightning and uses the receipt as auth.
- [Machine Payments Protocol (MPP)](https://github.com/tempoxyz/mpp-specs) - Tempo and Stripe spec for HTTP 402 payments through a Payment auth scheme.
- [Trusted Agent Protocol](https://github.com/visa/trusted-agent-protocol) - Visa spec that lets merchants verify a known agent is acting for a real shopper.
- [Trusted Agentic Commerce Protocol](https://github.com/forter/trusted-agentic-commerce-protocol) - Forter protocol that signs and encrypts agent data passed to merchants and vendors.
- [Universal Commerce Protocol (UCP)](https://github.com/Universal-Commerce-Protocol/ucp) - Open spec, started by Google, for catalog, cart, checkout and orders between agents and shops.
- [Verifiable Intent](https://github.com/agent-intent/verifiable-intent) - Mastercard draft for SD-JWT credentials that prove an agent stayed within user limits.
- [x402](https://github.com/x402-foundation/x402) - Open protocol that uses HTTP 402 so clients and agents can pay for resources in stablecoins.

## Payment networks and providers

- [Adyen Agentic](https://www.adyen.com/agentic-commerce) - Adyen integration for accepting payments that AI agents start for shoppers.
- [Checkout.com Agentic Commerce](https://www.checkout.com/agentic-commerce) - Checkout.com tools for merchants to take payments from purchases made by AI agents.
- [Cloudflare Pay per Crawl](https://developers.cloudflare.com/ai-crawl-control/features/pay-per-crawl/) - Cloudflare feature that charges AI crawlers a set price to fetch a site's pages.
- [Coinbase x402 Facilitator](https://docs.cdp.coinbase.com/x402/welcome) - Coinbase docs and hosted service for verifying and settling x402 payments.
- [Lithic Agentic Commerce](https://www.lithic.com/solutions/agentic-commerce) - Virtual card issuing for agents with spend controls and adaptive approvals.
- [Mastercard Agent Pay](https://www.mastercard.com/global/en/business/artificial-intelligence/mastercard-agent-pay.html) - Mastercard program that registers agents and gives them tokenized cards to pay with.
- [PayPal Agentic Commerce](https://www.paypal.ai/) - PayPal services that let merchants sell through AI agents and agents pay with PayPal.
- [Stripe Agentic Commerce](https://docs.stripe.com/agentic-commerce) - Stripe docs for selling through AI agents over ACP with delegated payment tokens.
- [Stripe Machine Payments](https://docs.stripe.com/payments/machine) - Stripe docs for charging agents per call or per request over MPP and x402.
- [Visa Intelligent Commerce](https://www.visa.com/en-us/solutions/intelligent-commerce) - Visa program for agent-ready tokenized cards, spend controls and authentication.

## Agent payment platforms

- [AgentCash](https://agentcash.dev/) - Merit Systems balance that lets agents pay per call for APIs without keys.
- [ATXP](https://atxp.ai/) - Agent accounts with a wallet, email and pay-per-use tools.
- [Catena](https://catena.com/) - Governance and banking platform for AI agents that hold and move money.
- [Crossmint](https://www.crossmint.com/solutions/agentic-payments) - Wallets, virtual cards and payouts that let agents buy online and onchain.
- [Kite](https://gokite.ai/) - Chain and identity layer built for agents to send and receive stablecoin payments.
- [Locus](https://paywithlocus.com/) - One agent account for many paid APIs and data sources, billed per call.
- [Natural](https://www.natural.co/) - Wallets, cards and payment processing for moving money between agents and people.
- [Nevermined](https://nevermined.ai/) - Lets agents delegate spending, meter usage and settle over MCP, x402 and A2A.
- [Payman](https://paymanai.com/) - AI agents that run payments and transfers on a bank's existing rails, with controls.
- [Skyfire](https://skyfire.xyz/) - Gives agents verified identity and payment credentials to pay sites and APIs.

## Shopping agents and storefronts

- [Amazon Buy for Me](https://www.aboutamazon.com/news/retail/amazon-shopping-app-buy-for-me-brands) - Amazon app feature where an agent buys items from other brands' sites for the shopper.
- [Channel3](https://trychannel3.com/) - Product graph and API that agents use to find products across many stores.
- [Claude for Commerce Examples](https://github.com/Shopify/claude-for-commerce-examples) - Shopify storefront and merchant agents built on Anthropic's commerce blueprint.
- [Commerce Agents](https://github.com/anthropics/commerce-agents) - Anthropic reference blueprint for shopping and merchant agents built on Claude.
- [commercetools Agentic Commerce](https://commercetools.com/products/agentic-commerce) - commercetools products for letting AI agents discover and buy from a store.
- [Crossmint Checkout Agent](https://github.com/Crossmint/crossmint-checkout-telegram-agent) - Telegram agent that buys Amazon products with a card or crypto.
- [Firmly](https://www.firmly.ai/) - Connects merchant catalogs and checkout to AI agents and other buying surfaces.
- [Google UCP Merchant Guide](https://developers.google.com/merchant/ucp) - Google guide for merchants to sell through AI Mode and Gemini over UCP.
- [Open Supermarkets](https://github.com/abracadabra50/open-supermarkets) - CLI, MCP server and skills to search, compare and check out at supermarkets.
- [OpenAI Commerce](https://developers.openai.com/commerce/) - OpenAI docs for merchants to sell through Instant Checkout in ChatGPT.
- [Perplexity Shopping](https://www.perplexity.ai/shopping) - Perplexity feature that finds products and checks out inside the chat.
- [Rye](https://www.rye.com/) - API that lets an AI app buy products from online stores in a native checkout.
- [Saleor Agentic Commerce](https://saleor.io/agentic-commerce) - Open-source commerce platform's support for selling through agents over ACP and AP2.
- [Shop Chat Agent](https://github.com/Shopify/shop-chat-agent) - Shopify template for a storefront chat agent that helps shoppers find and buy products.
- [Shopify Agentic Commerce Docs](https://shopify.dev/docs/agents) - Shopify docs for building agents that search catalogs and check out over UCP.
- [Shopify Agentic Storefronts](https://www.shopify.com/agentic-storefronts) - Shopify feature that puts merchant products on sale inside AI chats.
- [UCP CLI](https://github.com/Shopify/ucp-cli) - Shopify shopping skill that lets an agent browse and buy from UCP merchants.
- [Wildcard](https://wild-card.ai/) - Tracks and tunes how a store shows up on AI shopping surfaces.
- [Zinc](https://www.zinc.com/) - API that places, tracks and returns orders at many retailers for apps and agents.

## SDKs and tools

### Commerce protocol tooling

- [ACP Checkout Gateway](https://github.com/nekuda-ai/ACP-Checkout-Gateway) - Serverless reference gateway for Agentic Commerce Protocol checkout.
- [acp-handler](https://github.com/vercel/acp-handler) - Vercel library for serving Agentic Commerce Protocol endpoints from a server.
- [Magento 2 UCP Module](https://github.com/magebitcom/magento2-universal-commerce-module) - In-progress UCP implementation for Magento 2 and Adobe Commerce stores.
- [Retail Agentic Commerce](https://github.com/NVIDIA-AI-Blueprints/Retail-Agentic-Commerce) - NVIDIA reference build of ACP and UCP for retail shopping agents.
- [UCP Agent](https://github.com/Upsonic/UCP-Agent) - Upsonic shopping assistant that buys from merchants over UCP.
- [UCP Conformance](https://github.com/Universal-Commerce-Protocol/conformance) - Test suite that checks a UCP implementation against the spec.
- [UCP JavaScript SDK](https://github.com/Universal-Commerce-Protocol/js-sdk) - Official JavaScript SDK for building UCP merchants and agents.
- [UCP Python SDK](https://github.com/Universal-Commerce-Protocol/python-sdk) - Official Python SDK for building UCP merchants and agents.
- [UCP Samples](https://github.com/Universal-Commerce-Protocol/samples) - Sample shopping agents and merchant servers that speak UCP.
- [UCP Schema](https://github.com/Universal-Commerce-Protocol/ucp-schema) - Validator that checks UCP payloads against the protocol schemas.

### x402 and MPP

- [a2a-x402-typescript](https://github.com/dabit3/a2a-x402-typescript) - TypeScript port of the A2A x402 extension for paid calls between agents.
- [AgentCash Router](https://github.com/Merit-Systems/agentcash-router) - Server framework for building APIs that accept x402 and MPP payments.
- [Faremeter](https://github.com/faremeter/faremeter) - Plugin-based libraries and proxies that let agents pay over HTTP 402 on any chain.
- [MCPay](https://github.com/microchipgnu/MCPay) - Open-source tools and registry for charging for MCP server tools with x402.
- [mpp-rs](https://github.com/tempoxyz/mpp-rs) - Rust SDK for the Machine Payments Protocol.
- [mppx](https://github.com/wevm/mppx) - TypeScript library for clients and servers of the Machine Payments Protocol.
- [Pay](https://github.com/solana-foundation/pay) - Solana Foundation CLI that handles agent payments over x402, MPP and AP2.
- [Pay Kit](https://github.com/solana-foundation/pay-kit) - Solana Foundation building blocks for x402, MPP and AP2 payments in many languages.
- [PipeGate](https://github.com/Dhruv-2003/pipegate) - Pays for APIs with stablecoin channels and x402 instead of API keys.
- [qntx facilitator](https://github.com/qntx/facilitator) - Self-hosted server that verifies and settles x402 payments.
- [r402](https://github.com/qntx/r402) - Rust SDK for the x402 payment protocol.
- [x402 MCP](https://github.com/ethanniser/x402-mcp) - Helpers for paid MCP tools over x402 with the Vercel AI SDK.
- [x402 Proxy](https://github.com/cascade-protocol/x402-proxy) - CLI and MCP proxy that pays x402 and MPP endpoints on behalf of the caller.
- [x402 Rails](https://github.com/quiknode-labs/x402-rails) - Ruby on Rails gem for accepting x402 payments in an app.
- [x402 Starter Kit](https://github.com/dabit3/x402-starter-kit) - Starter project for building and deploying an x402 paid API.
- [x402-dotnet](https://github.com/michielpost/x402-dotnet) - .NET implementation of the x402 payment protocol.
- [x402-rs](https://github.com/x402-rs/x402-rs) - Rust crates and facilitator for verifying and settling x402 payments.
- [x402-solana](https://github.com/PayAINetwork/x402-solana) - PayAI library for x402 v2 payments from Solana clients and servers.

### Lightning and L402

- [Alby MCP](https://github.com/getAlby/mcp) - MCP server that connects a Lightning wallet to an agent through Nostr Wallet Connect.
- [Aperture](https://github.com/lightninglabs/aperture) - Lightning Labs reverse proxy that charges for API calls with L402.
- [L402 SDK](https://github.com/lightninglabs/L402sdk) - Client SDK for agent frameworks to pay L402 APIs over Lightning.
- [Lightning Agent Tools](https://github.com/lightninglabs/lightning-agent-tools) - Skills and MCP server for agents to run nodes and pay for or host L402 APIs.
- [lnget](https://github.com/lightninglabs/lnget) - wget-style CLI that pays for L402 requests with Lightning.
- [ngx-l402](https://github.com/ngx-l402/ngx-l402) - nginx module that puts API routes behind L402 payments.

### Agent wallets and toolkits

- [Agentic Wallet Skills](https://github.com/coinbase/agentic-wallet-skills) - Coinbase skills that let coding agents hold a wallet, send funds and pay.
- [AgentKit](https://github.com/coinbase/agentkit) - Coinbase toolkit that gives agents crypto wallets and onchain actions.
- [AgentPay SDK](https://github.com/worldliberty/agentpay-sdk) - SDK and CLI for agents to pay by card through Link or from a local crypto wallet.
- [Bindu](https://github.com/GetBindu/Bindu) - Framework that adds identity, agent-to-agent messaging and x402 payments to agents.
- [ClawRouter](https://github.com/BlockRunAI/ClawRouter) - LLM router where agents pay for each model call from one USDC wallet.
- [Link CLI](https://github.com/stripe/link-cli) - Stripe CLI that lets agents spend from a Link wallet after the user approves each purchase.
- [Lucid Agents](https://github.com/daydreamsai/lucid-agents) - Commerce SDK for agents that pay, sell and trade services with other agents.
- [MoonPay Skills](https://github.com/moonpay/skills) - Skills for agents to on-ramp, swap and move funds through the MoonPay CLI.
- [PayPal Agent Toolkit](https://github.com/paypal/agent-toolkit) - Library that exposes PayPal APIs as tools for agent frameworks and MCP.
- [Steward](https://github.com/Steward-Fi/steward) - Self-hosted wallet and credential proxy with spend policy and approvals for agents.
- [Stripe AI](https://github.com/stripe/ai) - Stripe agent toolkit and MCP server for calling Stripe APIs from agents.
- [Visa AI Toolkit](https://github.com/visa/ai) - Toolkit for connecting AI agents to Visa Intelligent Commerce.

## Discovery and directories

- [Agentic Market](https://agentic.market/) - Directory of services agents can pay for over x402 without API keys.
- [Coinbase x402 Bazaar](https://docs.cdp.coinbase.com/x402/bazaar) - Discovery layer that lists x402 services for agents to find and pay.
- [UCP Checker](https://ucpchecker.com/) - Validator that checks a store's UCP profile and reports its status.
- [x402scan](https://github.com/Merit-Systems/x402scan) - Explorer for x402 transactions, sellers and paid resources.

## Benchmarks and research

- [ACES](https://github.com/mycustomai/ACES) - Sandbox for studying how vision-language agents shop and pick products online.
- [CommerceAgentBench](https://github.com/Accio-org/CommerceAgentBench) - Alibaba benchmark of long agent tasks in replicas of real commerce services.
- [E-CommerceBench](https://github.com/QwenLM/E-CommerceBench) - Qwen benchmark where LLM agents run simulated online stores for a year.
- [Magentic Marketplace](https://github.com/microsoft/multi-agent-marketplace) - Microsoft simulation of markets where buyer and seller agents transact.
- [MerchantBench](https://github.com/KhanCold/merchantbench) - Year-long benchmark of LLM agents running seller-side store operations.

## Guides

- [ACP Website](https://www.agenticcommerce.dev/) - Overview and docs for the Agentic Commerce Protocol.
- [Announcing AP2](https://cloud.google.com/blog/products/ai-machine-learning/announcing-agents-to-payments-ap2-protocol) - Google Cloud post that introduced the Agent Payments Protocol.
- [AP2 Documentation](https://ap2-protocol.org/) - AP2 spec, core concepts and a walkthrough of one transaction.
- [Buy It in ChatGPT](https://openai.com/index/buy-it-in-chatgpt/) - OpenAI post that launched Instant Checkout and the Agentic Commerce Protocol.
- [Cloudflare Agents x402 Guide](https://developers.cloudflare.com/agents/agentic-payments/x402/) - Guide to charging for and paying for resources with x402 in Cloudflare Agents.
- [Copilot Checkout and Brand Agents](https://about.ads.microsoft.com/en/blog/post/january-2026/conversations-that-convert-copilot-checkout-and-brand-agents) - Microsoft post on buying inside Copilot and on brand agents.
- [Developing an Open Standard for Agentic Commerce](https://stripe.com/blog/developing-an-open-standard-for-agentic-commerce) - Stripe post on why and how ACP was designed.
- [Introducing the Machine Payments Protocol](https://stripe.com/blog/machine-payments-protocol) - Stripe post that introduced MPP for payments by agents.
- [L402 Documentation](https://docs.lightning.engineering/the-lightning-network/l402) - Lightning Labs docs on how L402 pays for and authenticates API calls.
- [MPP Documentation](https://mpp.dev/) - Docs for the Machine Payments Protocol from Tempo and Stripe.
- [Secure Use of AP2](https://cloudsecurityalliance.org/blog/2025/10/06/secure-use-of-the-agent-payments-protocol-ap2-a-framework-for-trustworthy-ai-driven-transactions) - Cloud Security Alliance framework for deploying AP2 safely.
- [UCP Documentation](https://ucp.dev/) - Spec, guides and playground for the Universal Commerce Protocol.
- [Under the Hood of UCP](https://developers.googleblog.com/under-the-hood-universal-commerce-protocol-ucp/) - Google Developers post on how UCP is designed.
- [x402 Documentation](https://docs.x402.org/) - Docs for the x402 protocol, its SDKs and facilitators.
- [x402 Foundation Announcement](https://blog.cloudflare.com/x402/) - Cloudflare post on forming the x402 Foundation with Coinbase.
- [x402 Whitepaper](https://www.x402.org/x402-whitepaper.pdf) - Paper that sets out the design and motivation behind x402.

## Related lists

- [Awesome Agent Payments Protocol](https://github.com/tsubasakong/awesome-agent-payments-protocol) - Resources on AP2, A2A and x402.
- [Awesome Agentic Commerce (damoahdominic)](https://github.com/damoahdominic/awesome-agentic-commerce) - Protocol deep dives, platforms and reading on agentic commerce.
- [Awesome Agentic Commerce (MentionNetwork)](https://github.com/MentionNetwork/awesome-agentic-commerce) - Protocols, MCP servers, apps and APIs for agent shopping.
- [Awesome Agentic Commerce (Merit Systems)](https://github.com/Merit-Systems/awesome-agentic-commerce) - x402-focused list of specs, SDKs, facilitators and examples.
- [Awesome Agentic Commerce (xpaysh)](https://github.com/xpaysh/awesome-agentic-commerce) - Protocol comparison and platform plugins for ACP, UCP and AP2.
- [Awesome L402](https://github.com/Fewsats/awesome-L402) - Tools, libraries and services built on L402.
- [Awesome UCP](https://github.com/Upsonic/awesome-ucp) - Resources, tools and implementations for the Universal Commerce Protocol.
- [Awesome x402](https://github.com/xpaysh/awesome-x402) - Resources for x402 payments, facilitators and paid APIs.

## Contributing

Contributions are welcome. Read the [contribution guidelines](contributing.md) first.

<!-- awesome:maintainer -->
Maintained by [Ian Wiedenman](https://github.com/ianwieds).
<!-- /awesome:maintainer -->

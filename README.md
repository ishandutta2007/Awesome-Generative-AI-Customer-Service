# Awesome-Generative-AI-Customer-Service

# Top Generative AI Customer Service Ecosystem

**Curated List of SaaS Platforms & Open-Source GitHub Projects**  
*Focused on Agentic Support Automation, RAG-Grounded Resolution & Self-Hosted Customer Service Engines*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Generative AI Customer Service**. These tools help support teams deploy AI agents that resolve inquiries, draft responses, and escalate to humans when confidence is low—covering everything from polished commercial copilots embedded in helpdesks to open-source frameworks that let you build and self-host your own support agent stack.

**Examples** include Intercom Fin, Salesforce Agentforce, Freshworks Freddy AI, Zendesk Generative AI, Ada, Decagon, Sierra AI, and open-source alternatives like Upsonic, LibreChat, and Tiledesk (the category leaders).

**Open-source emphasis**: This section highlights every major active project for self-hosted AI customer service, open-source agent frameworks, and community-driven support automation—ideal for organizations seeking data sovereignty and avoiding per-resolution or per-seat SaaS pricing. The open-source landscape is genuinely functional: **Upsonic** provides a production-ready agent framework with a Safety Engine for compliance , **LibreChat** offers a self-hosted multi-provider AI platform with MCP support and enterprise SSO , and **FastGPT** delivers an Apache 2.0 knowledge-base Q&A system with visual workflow orchestration .

Contributions welcome! Open an PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

| Product | Description | Pricing (Starting) | Free Tier / Trial Limits |
|---------|-------------|-------------------|--------------------------|
| **[Intercom Fin](https://www.intercom.com/)** | AI agent that resolves conversations autonomously at **$0.99 per outcome**. Copilot assists human agents with drafting and knowledge retrieval. | Fin outcomes: **$0.99 each**; Essential: **$29/seat/month** (annual) | No permanent free tier; trial available |
| **[Salesforce Agentforce](https://www.salesforce.com/)** | AI agent platform embedded across Salesforce for service, sales, and marketing. Grounded in CRM data via the Einstein Trust Layer. | Quote-only (bundled with Salesforce licensing; per-conversation pricing available) | No free tier; demo via sales |
| **[Freshworks Freddy AI](https://www.freshworks.com/)** | Generative AI for customer service within Freshdesk and Freshservice. Freddy AI Agent resolves routine requests before they reach human agents. | Quote-only (bundled with Freshworks plans) | No free tier; trial via sales |
| **[Zendesk Generative AI](https://www.zendesk.com/)** | AI assistant within Zendesk that suggests responses, summarizes tickets, and surfaces knowledge. | Quote-only (bundled with Zendesk Suite) | No free tier; trial via sales |
| **[Ada](https://www.ada.cx/)** | AI-powered customer service automation platform. Automates resolutions across chat, voice, and email with no-code AI agent building. | Quote-only | No free tier; demo via sales |
| **[Decagon](https://decagon.ai/)** | AI customer support agent positioned for high-growth tech companies. Focused on accurate, grounded responses with human handoff. | Quote-only | No free tier; demo via sales |
| **[Sierra AI](https://sierra.ai/)** | Conversational AI platform for customer service, founded by Bret Taylor. Positioned for enterprise deployments with branded agents. | Quote-only | No free tier; demo via sales |

## Open-Source GitHub Projects

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[Upsonic](https://github.com/Upsonic/Upsonic)** | — | **The most production-oriented open-source agent framework with a built-in Safety Engine.** Used by fintech companies, banks, and developers worldwide for **customer service automation, document analysis, and multi-agent workflows** [citation:3][citation:10]. **Safety Engine**: pre-built policies for **PII blocking, content filtering**, custom compliance policies, real-time monitoring, and detailed audit logs—LLM-agnostic and production-ready . **Memory management** for context-aware conversations, **OCR support**, **MCP tool integration**, and **human-in-the-loop workflows** [citation:15]. **Best for teams wanting a production-grade agent framework** with compliance controls built in . |
| **[LibreChat](https://github.com/danny-avila/LibreChat)** | — | **The most widely adopted self-hosted multi-provider AI platform with agent capabilities.** **MIT licensed, 46.9k GitHub stars** [citation:4]. **Unified interface for OpenAI, Anthropic, Google, Azure, AWS Bedrock, and dozens more**—no vendor lock-in. **MCP support, custom endpoints, plugins, and agents**—administrators control which MCP servers are available; users build agents on those servers without code and share them through a marketplace [citation:11]. **Enterprise-ready**: SSO (OAuth, SAML, LDAP), two-factor auth, rate limiting, and moderation tools. **Thoughtworks Trial rating**: a team built a client's internal AI platform on LibreChat with MCP servers for Jira, Confluence, Salesforce, and internal systems—sales built agents to check availability and book orders [citation:11]. **Best for organizations wanting a self-hosted, multi-model agent platform** with enterprise auth and a proven deployment pattern . |
| **[FastGPT](https://github.com/labring/FastGPT)** | — | **The most complete open-source knowledge-base Q&A system with visual workflow orchestration.** **Apache 2.0 licensed**, TypeScript/Next.js, Docker deployment [citation:6]. **RAG-powered intelligent customer service** with multi-model support and multi-turn dialogue with context memory [citation:13]. **Flow module** enables visual workflow orchestration; **open API** integrates with CRM/ERP systems [citation:6]. **Knowledge-base closed-loop**: records unanswered questions for content optimization, supports user thumbs up/down feedback to tune retrieval thresholds [citation:13]. **Best for teams wanting a self-hosted RAG-based customer service knowledge base** with workflow automation . |
| **[Tiledesk](https://github.com/Tiledesk/tiledesk-server)** | — | **Open-source LLM agent platform with visual conversation flow design and human-in-the-loop handoff.** Node.js microservices architecture with Docker Compose or Kubernetes deployment [citation:7]. **Built-in AI**: LLM-powered agent building is the core product—visually design automated answers and human handoff points [citation:7]. **Model choice**: built around LLM integrations; check docs for supported providers. **Hosted cloud option available** [citation:7]. **Best for teams wanting to design multi-step agent workflows** rather than install a ready-made support agent . |
| **[recourse](https://github.com/ibrahimhajjaj/recourse)** | — | **The most feature-complete self-hosted AI customer support agent with help desk included.** **Answers from your content**: crawls sites, reads folders (PDFs, Word, slides, spreadsheets, EPUB), imports Notion. **Hybrid retrieval** (keyword + vector) degrades gracefully to keyword-only without embeddings [citation:9]. **Acts, not just replies**: captures leads, calls APIs, looks up Stripe subscriptions or Shopify orders, escalates to humans [citation:9]. **Runs a help desk**: tickets with statuses, teams, routing rules, assignment, AI-drafted replies a person approves before sending [citation:9]. **Multi-channel**: Web widget, WhatsApp, Messenger, Instagram, Slack, Telegram, Discord, SMS, email—each checking platform signatures [citation:9]. **Answers the phone** via Twilio or ElevenLabs [citation:9]. **Refuses instruction-override attempts** before reaching the model; **records unanswered questions** ranked as content gaps [citation:9]. **Best for teams wanting a complete self-hosted support stack** from AI agent to help desk to multi-channel . |
| **[Rasa](https://github.com/RasaHQ/rasa)** | — | **The most mature open-source conversational AI framework** with 25M+ downloads [citation:5]. **NLU, dialogue management, and integrations** with messaging channels. **Trade-off**: Rasa Pro (commercial) adds security, observability, and scale—the open-source edition is the foundation, not the full enterprise product [citation:5]. **Best for teams wanting a proven conversational AI foundation** with full control over dialogue logic . |

### Additional Strong Open-Source Options

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[openagent](https://github.com/skoopplayz/openagent)** | — | **Free open-source customer service agent designed to be embedded on websites.** Single-script embed with Llama 3.2 70B API integration. **Trade-off**: widget status noted as broken in README, though HTML demo works [citation:2]. **Best as a lightweight starting point** for embedded support agents . |
| **[agentic-ai-customer-support](https://github.com/Thekeshavjoshi/agentic-ai-customer-support)** | — | **Agentic customer support with tool calling, RAG, and persistent memory.** Groq-powered LLM + FAISS vector store + Gradio interface. Tools: calculator, order tracking, knowledge base search. **Conversational memory** maintains context across interactions [citation:14]. **Best as a reference implementation** for tool-calling support agents with RAG . |

**Frameworks for building custom systems**: Choose **Upsonic** for a production agent framework with Safety Engine and PII blocking , **LibreChat** for a self-hosted multi-model agent platform with MCP and enterprise SSO , **FastGPT** for a RAG-based knowledge-base Q&A system with visual workflows , or **recourse** for a complete self-hosted support stack including help desk and multi-channel—all without per-resolution or per-seat SaaS fees.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- AI customer service platforms process customer conversations and potentially sensitive PII; enforce **prompt-injection defenses** (recourse refuses instruction-override attempts before reaching the model [citation:9]), **PII blocking** (Upsonic's Safety Engine [citation:3]), and **human-in-the-loop review** for consequential actions like refunds [citation:1].
- **Open-source customer service tooling has different maturity levels and trade-offs.** **Upsonic is the most production-oriented agent framework** with built-in compliance controls, but requires engineering to deploy and customize [citation:3][citation:10]. **LibreChat is the most widely adopted self-hosted AI platform** (46.9k stars, Thoughtworks Trial) with a proven pattern of building MCP servers for internal systems and letting non-engineers build agents —but it's a platform, not a turnkey support agent [citation:4][citation:11]. **FastGPT is the most complete knowledge-base Q&A system** with RAG and workflows, but documentation is primarily Chinese [citation:6]. **recourse is the most complete self-hosted support stack**—agent + help desk + multi-channel—but is newer and less proven than commercial platforms [citation:9]. **Tiledesk pivoted from live chat to LLM agent flows**, making it suitable for teams wanting visual conversation design rather than a ready-made agent [citation:7]. **Commercial platforms (Intercom Fin, Ada, Decagon, Sierra) bundle seamlessly into their ecosystems** but charge per-resolution ($0.99/outcome for Fin) or require full platform subscriptions. **Validate whether you need a turnkey SaaS agent (Fin, Ada), a self-hosted agent platform (LibreChat, Upsonic), a RAG knowledge base (FastGPT), or a complete support stack (recourse)** before committing.

---

**Made for support operations leaders, AI engineers, and organizations building agentic customer service.**  
Let's make generative AI customer service more open, grounded, and controllable.

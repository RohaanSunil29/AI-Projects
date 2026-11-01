# Where AI agents are heading: 12-24 month outlook from October 2026

Notes as of 2026-10-30.

**Labels used on every item**
- **[SOLID]** = shipped, measured, legally in force, or an adopted standard.
- **[SOLID, vendor claim]** = the event is real, but the number or description comes from the party that benefits. No independent check was found.
- **[SPECULATION]** = forecast, prediction, or extrapolation.

**Evidence markers**
- No marker = I read the page.
- **(snippet)** = I saw only a search excerpt or digest. Verify before quoting.

**Citation format:** [Title](URL) (publisher, publication date). "n.d." means no date was visible in what I retrieved.

**Disclosure:** these notes were written by a Claude model, so treat Anthropic items with the same vendor-claim caution as other labs.

## What measured trends point forward, and how reliable is extending them?

### Takeaway
Task capability and price-for-fixed-performance are both moving fast, and they are the best-evidenced trends available. But the flagship capability chart has hit its ceiling: METR says readings above 16 hours are unreliable, and its page has had no model added since May 2026. So the capability trend is now weakest exactly where the next two years matter. Cost per fixed performance falls about 13x a year, but cost per frontier agent workflow is forecast to rise, and both can be true at once.

### Cited Findings

**Capability (time horizon)**
- [SOLID] METR's revised TH1.1 method gives a post-2023 doubling time of 131 days (165 days under TH1), and 89 days since 2024. The original 2025 paper estimated about 7 months for 2019-2024. — [Time Horizon 1.1](https://metr.org/blog/2026-01-29-time-horizon-1-1/) (METR, 2026-01-29) (snippet)
- [SOLID] METR's tracker warns "Measurements above 16 hrs are unreliable with our current task suite." It was last updated 2026-09-08 and described as no longer actively updated. The newest models listed are Claude Mythos Preview (early, added 2026-05-08), Gemini 3.1 Pro (2026-04-15) and GPT-5.4 (2026-04-10). — [Time Horizons](https://metr.org/time-horizons/) (METR, updated 2026-09-08)
- [SOLID] Early Claude Mythos Preview: 50% horizon about 17 hours (95% CI about 8.5-55 hours), 80% horizon about 3h06m. METR's tracker itself gave no numbers in the text I retrieved. — [METR](https://en.wikipedia.org/wiki/METR) (Wikipedia, n.d.) (snippet)
- [SOLID] Public frontier, February-March 2026: 50% horizon about 12 hours (range 5-61 hours), 80% horizon about 1.5 hours. METR estimated the internal frontier was about 66 days ahead of the public trend. — [Frontier Risk Report](https://metr.org/blog/2026-05-19-frontier-risk-report/) (METR, 2026-05-19) (snippet)
- [SOLID] The 50% and 80% figures differ by roughly 5-8x. An agent that "can do" a 12-17 hour task succeeds about half the time. The 80% figure is the better guide for unattended work. — same sources as the two items above
- [SOLID] METR's own researcher notes that as models improve "many of the human-relevant benchmarks become no longer useful." He surveys replacements: continuous horizon, expenditure horizon, and "nines of reliability." — [Metrics of Agent Ability](https://metr.org/notes/2026-07-24-metrics-of-model-ability/) (METR, Tom Cunningham, 2026-07-24)
- [SOLID] Criticism of the chart: small sample at the frontier, public task topics that labs can train toward, and estimated rather than measured human baselines for most long tasks. This comes from a parody that applies the method to Excel. It is **not a METR release despite the "Time Horizon 2.0" title**. A commenter who authored METR's limitations post said most of the criticisms are already known. — [METR Time Horizon 2.0](https://forum.effectivealtruism.org/posts/ghhJh6SBYXxDktnZX/metr-time-horizon-2-0-the-benchmark-you-ve-been-waiting-for) (EA Forum, AgentMa, 2026-07-08; flagged by the forum as AI-written)
- Source conflict: Claude Opus 4.6 is reported as both 14.5 hours and 718 minutes in secondary trackers (snippet; [agitracker](https://agitracker.io/blog/metr-time-horizons-2026/), n.d.). This is unresolved, so avoid citing either figure.

**Real-world productivity versus benchmarks**
- [SOLID] METR's early-2025 study found AI lengthened task times for experienced open-source developers (CI +2% to +39%). — [early-2025 study](https://metr.org/blog/2025-07-10-early-2025-ai-experienced-os-dev-study/) (METR, 2025-07-10) (snippet)
- [SOLID] METR's follow-up gave about -18% task time for returning developers and -4% for new ones, with both intervals crossing zero. METR called the signal unreliable because of selection: the study is missing the developers with the most optimistic expectations about AI. It is redesigning the study. Its statement that developers are likely faster now is qualitative. Blogs reporting "18% faster" overstate this. — [Uplift update](https://metr.org/blog/2026-02-24-uplift-update/) (METR, 2026-02-24) (snippet)

**Benchmarks**
- [SOLID] Stanford AI Index 2026 as reported secondhand: OSWorld computer tasks about 12% to 66.3% in a year; Terminal-Bench 20% to 77.3%; Cybench 15% (2024) to 93% (2025). Many benchmarks reportedly have 20-40% error rates. — [Stanford AI Index 2026 coverage](https://www.beri.net/article/stanford-ai-index-2026-agents-66-percent-success) (BERI, n.d.) (snippet). I did not reach the primary report. The same headline's "89% never reach production" could not be traced to Stanford, so do not use it.

**Cost**
- [SOLID] The cost of a fixed performance level fell about 47% per quarter (about 13x a year) since 2023. That is 39-43% per quarter on game puzzles and 50-52% on math. Costs fall fastest right after a level becomes state of the art: 66% per quarter at the frontier, 32% two years later. Example: 75% on GPQA Diamond cost about $0.30 per question with o3 (January 2025) and $0.0004 with GPT-5.6 Luna. — [The Plunging Price of Thought](https://epoch.ai/publications/the-plunging-price-of-thought) (Epoch AI, Emberson and Roodman, 2026-09-22)
- [SOLID] Epoch's caveats: it tracks the cheapest model reaching a level, not total spending. It assumes users always switch to the cheapest model. Reasoning models use many more tokens. The data covers barely three years. Benchmarks can be gamed. Epoch makes no forecast.
- [SPECULATION] Gartner predicts AI inference costs per agentic workflow will rise more than fivefold through 2028. Routing a task to an agentic reasoning model costs at least 5x a basic chatbot interaction, "often much more." — [Gartner release](https://www.gartner.com/en/newsroom/press-releases/2026-08-17-gartner-predicts-ai-inference-costs-per-agentic-workflow-will-increase-more-than-fivefold-through-2028) (Gartner, 2026-08-17)
- Apparent disagreement: Epoch (13x cheaper per year) versus Gartner (5x dearer per workflow). They measure different things, fixed performance versus moving frontier workflows. Gartner's own text agrees that token economics are improving. The disagreement is real only if someone reads Epoch as "your bill will fall."

**Release pace**
- [SOLID] Dated model names show a fast cadence in 2026: GPT-5.4, Gemini 3.1 Pro and Mythos Preview in April-May ([METR tracker](https://metr.org/time-horizons/)); Gemini 3.5 at I/O in May ([TNW](https://thenextweb.com/news/google-gemini-spark-agentic-assistant-gmail-io-2026), n.d.) (snippet); Opus 5, Opus 5.5 and Sonnet 5.5 listed by Anthropic ([support page](https://support.claude.com/en/articles/8606394-how-large-is-the-context-window-on-paid-claude-plans), n.d.) (snippet); GPT-5.6 Luna ([Epoch](https://epoch.ai/publications/the-plunging-price-of-thought)). METR's homepage lists risk assessments for "Claude Opus 5.5" and "GPT-5.6 Sol" ([METR](https://metr.org/), n.d.) (snippet).

### Inferences
- [SPECULATION] My arithmetic, using a May 2026 base of 17 hours at the 50% level, for illustration only:
  - 7-month doubling: about 56 hours after 12 months, about 184 hours after 24 months.
  - 4-month doubling: about 136 hours after 12 months, about 1,090 hours (about 27 work weeks) after 24 months.
  - The 7-month and 4-month paths are about 6x apart at 24 months, so the choice of doubling time matters more than the base.
  - None of these figures could be checked with the current suite, so any claim of "weeks-long agents" by 2028 is unmeasured extrapolation.
- Extending the time-horizon trend is moderately reliable as a direction and weak as a magnitude. Reasons: the suite is saturated, the 89-day recent rate rests on a short window, tasks are clean and self-contained, and reliability is far lower than the headline.
- Extending the price trend is more reliable for routine tasks than for frontier tasks. Epoch's decay slowing by age suggests buyers on cheaper tiers capture most of the decline, while heavy frontier users do not.
- The most useful practical number is the 80% horizon of about 1.5-3 hours, not the 50% headline.

### Gaps
- No public METR time horizon was found for any model after Mythos Preview (including Opus 5, Opus 5.5 and GPT-5.6). I could not confirm whether METR has a replacement suite coming.
- No source directly measures release cadence, such as median days between frontier releases.
- No independent cost-per-completed-agent-task series was found. Toby Ord's EA Forum post "Are the Costs of AI Agents Also Rising Exponentially?" was seen by title only and is a lead worth checking.
- Stanford's primary report was not retrieved.

## What infrastructure is being adopted, and what do adoption figures show?

### Takeaway
Standards consolidation is the most solid story in this field: MCP, A2A, AGENTS.md and Agent Skills now share one Linux Foundation home. But nearly every adoption number comes from the projects or their backers and measures SDK downloads or logos, not production use. Agent payments are the clearest case of infrastructure outrunning demand. Skills marketplaces are the clearest new security risk.

### Cited Findings

**Governance**
- [SOLID] The Agentic AI Foundation launched 2025-12-09 with MCP (Anthropic), goose (Block) and AGENTS.md (OpenAI). — [LF press release](https://www.linuxfoundation.org/press/linux-foundation-announces-the-formation-of-the-agentic-ai-foundation) (Linux Foundation, 2025-12-09) (snippet)
- [SOLID] Membership grew to 146 in February 2026 ([AAIF](https://aaif.io/press/agentic-ai-foundation-welcomes-97-new-members-as-demand-for-open-collaborative-agent-standardization-increases), 2026-02) (snippet), 190 in May ([LF](https://www.linuxfoundation.org/press/agentic-ai-foundation-adds-43-new-members-as-enterprise-and-government-adoption-of-open-agent-standards-accelerates), 2026-05) (snippet), and 305 by 2026-10-22 ([AAIF](https://aaif.io/news/agentic-ai-foundation-surpasses-300-members), 2026-10-22). Note: the 2026-10-22 release says 60 new members in its summary, but its body lists 58.
- [SOLID] On 2026-10-22 AAIF added Agent Skills (Anthropic), Open Responses (OpenAI), OpenEnv (Hugging Face) and OpenSandbox (Alibaba), taking it from 3 to 10 projects. The release gives no usage metrics. — [LF press release](https://www.linuxfoundation.org/press/agentic-ai-foundation-announces-four-new-projects-agent-skills-open-responses-openenv-and-opensandbox) (Linux Foundation, 2026-10-22)

**MCP**
- [SOLID, vendor claim] 97M+ monthly SDK downloads and 10,000 active servers. — [MCP joins AAIF](https://blog.modelcontextprotocol.io/posts/2025-12-09-mcp-joins-agentic-ai-foundation/) (MCP blog, 2025-12-09) (snippet)
- [SOLID, vendor claim] 110M monthly SDK downloads, stated by co-creator David Soria Parra in an April 2026 keynote. — [Dev Summit readout](https://www.digitalapplied.com/blog/mcp-dev-summit-2026-readout-protocol-roadmap-analysis) (Digital Applied, 2026-06) (snippet)
- [SOLID] The 2026-07-28 spec revision makes the protocol core stateless and adds an Extensions framework, Tasks, MCP Apps and authorization hardening. Tasks later moved to an extension. — [Release candidate](https://blog.modelcontextprotocol.io/posts/2026-07-28-release-candidate/) (MCP blog, n.d.; RC locked 2026-05-21) (snippet); [Python SDK v2 beta](https://github.com/modelcontextprotocol/python-sdk/releases/tag/v2.0.0b1) (GitHub, n.d.) (snippet). I could not confirm final publication.
- Moving from 97M (December 2025) to 110M (April 2026) is only a two-point comparison of rounded vendor figures, so it supports no conclusion about the growth rate.

**A2A**
- [SOLID] A2A launched April 2025, was donated to the Linux Foundation in June 2025, reached v1.0 in March 2026 (signed agent cards, multi-tenancy), and moved into AAIF on 2026-08-17. This changes the host, not who controls it. — [Forbes](https://www.forbes.com/sites/janakirammsv/2026/08/19/agent2agent-joins-the-agentic-ai-foundation-alongside-mcp/) (Forbes contributor Janakiram MSV, 2026-08-19). This resolves conflicting blog dates (August 20; "June 2025 donation").
- [SOLID, vendor claim] 150+ supporting organizations; support in Google Cloud, Azure AI Foundry and AWS Bedrock AgentCore; Huawei's HarmonyOS assistant uses it. Forbes notes the figures come from the foundation and vendors, and that implementation depth "varies widely." — same source
- [SOLID] IBM's ACP merged into A2A in August 2025. Cisco's AGNTCY still overlaps. — same source

**AGENTS.md and Agent Skills**
- [SOLID, vendor claim] AGENTS.md: 60,000+ open-source projects, attributed to OpenAI. — [Intuition Labs](https://intuitionlabs.ai/articles/agentic-ai-foundation-open-standards) (n.d.) (snippet; exact page attribution unclear)
- [SOLID] Agent Skills: published as an open standard December 2025; agentskills.io lists 40+ adopting clients (checked September 2026). — [Atlan](https://atlan.com/know/ai-agent/ai-agent-skills/what-are-agent-skills/) (n.d.) (snippet)
- [SOLID] One guide counts 490,000+ skills across three marketplaces as of March 2026. — [Virtual Uncle](https://virtualuncle.com/agent-skills-marketplace-skills-sh-2026/) (n.d.) (snippet; a raw count, and likely includes many duplicates)
- [SOLID] Security audits, as reported secondhand: Koi Security found 341 malicious skills out of 2,857 on ClawHub; the ClawHavoc campaign was reported at 1,184 malicious skills; Snyk found 36.82% of 3,984 skills had at least one flaw and 13.4% had a critical issue. Skills run with the host agent's privileges. — [AI Agent Skills: The New Supply Chain Risk](https://www.prplbx.com/blog/agent-skills-supply-chain) (n.d.) (snippet); [MalSkills](https://arxiv.org/pdf/2603.27204) (arXiv, 2026-03) (snippet). The digest did not map each figure to one URL, so trace originals before quoting. Counts differ by method.
- [SOLID] The OWASP Agentic Skills Top 10 exists and ranks malicious skills first. — [OWASP](https://github.com/OWASP/www-project-agentic-skills-top-10) (n.d.) (snippet)

**Browser and OS agents**
- [SOLID] Gemini Spark can drive desktop Chrome with signed-in accounts and saved passwords. It is US-first, and payments and sensitive actions need approval. — [9to5Google](https://9to5google.com/2026/07/30/gemini-spark-chrome-auto-browse/) (9to5Google, 2026-07-30) (snippet). Another source dates the US rollout to 2026-08-03; unresolved.
- [SOLID] Apple's App Intents is reported as the route for third-party apps to reach Siri, with SiriKit deprecated. — [Tech Times](https://www.techtimes.com/articles/318005/20260608/wwdc-2026-app-intents-replaces-sirikit-gemini-siri-migration-clock-starts.htm) (2026-06-08) (snippet). Secondary only.
- [SOLID, vendor claim] OS-level agent UI: Android Halo, a surface for agent progress, is "coming later this year." — [I/O keynote](https://blog.google/innovation-and-ai/sundar-pichai-io-2026/) (Google, 2026-05) (snippet)
- [SOLID] Prompt injection remains open. OpenAI reportedly said in December 2025 that it "may never be fully solved," then added Lockdown Mode in February 2026. — [Vectra](https://www.vectra.ai/topics/prompt-injection) (vendor, n.d.) (snippet; OpenAI's wording not verified). Researchers report mitigation, but [a 2026 paper](https://arxiv.org/pdf/2606.05233) (arXiv, 2026-06) (snippet) is among many still auditing it.

**Payments**
- [SOLID] OpenAI's Instant Checkout launched September 2025 and was retired in March 2026, with merchants returning to their own checkout. — [CNBC](https://www.cnbc.com/2026/03/20/open-ai-agentic-shopping-etsy-shopify-walmart-amazon.html) (CNBC, 2026-03-20) (snippet); [Exploding Topics](https://explodingtopics.com/blog/agentic-commerce-protocol) (n.d.) (snippet)
- [SOLID] Walmart found in-chat purchases converted at about a third of the rate of redirects to its own site. Etsy called volume relatively low. — [CNBC](https://www.cnbc.com/2026/03/20/open-ai-agentic-shopping-etsy-shopify-walmart-amazon.html) (snippet)
- Merchant go-live claims vary: about a dozen to about 30 merchants, or "about 30 Shopify stores." — [Digital Applied](https://www.digitalapplied.com/blog/ai-agentic-commerce-discover-in-ai-buy-on-site-2026) (n.d.) (snippet)
- [SOLID, vendor claim] Mastercard Agent Pay added a probability score for whether an agent initiated a transaction on 2026-10-01, in US testing. Trade press counted eight live protocols. No transaction volumes or primary links given. — [Contra Collective](https://contracollective.com/blog/agentic-payments-protocols-mastercard-visa-stripe-2026) (2026-10)
- Unverified: AP2 reportedly moved to the FIDO Alliance in April 2026 ([Reactify](https://www.reactify-solutions.com/articles/agentic-commerce-protocols-2026), n.d.) (snippet; the digest did not tie this claim to one URL). Sources conflict on whether ACP is a live product or just a surviving spec.
- Conflicting traffic figures: AI-referred retail traffic is reported as +693% YoY (2025 holidays) and +393% YoY (Q1 2026), and ChatGPT sessions as converting at 15.9%. These are different metrics, none verified. — [Koji](https://www.koji.so/blog/agentic-commerce-research-2026) (n.d.) (snippet)

### Inferences
- MCP is effectively settled as the tool-connection layer. A2A has governance but thinner evidence of real use. Small teams should prefer MCP now and treat A2A as something platforms handle for them.
- The pattern in commerce is discovery moving to agents while checkout stays with merchants. For small sellers, being findable and having clean product data matters before any payment protocol does.
- Skills are becoming an important distribution unit, and also a supply-chain risk, because they inherit an agent's permissions. Expect signing and registry vetting to become the visible next step (speculation).

### Gaps
- No independent measure of MCP or A2A production usage exists in what I found.
- No download figure later than April 2026.
- No transaction volumes for any agent payment protocol.
- Primary Visa, Mastercard, Google and FIDO announcements were not retrieved.
- No adoption statistics for consumer use of browser agents.

## What are the major labs and platforms shipping or committing to for consumers and small teams?

### Takeaway
Between May and October 2026, Google, Apple and Meta all shipped consumer agent products, alongside OpenAI's and Anthropic's existing agent tools. I found no comparable Microsoft consumer launch. Entry pricing clusters around $20 a month, with limits. Most are US-first, capped, or labelled beta, so reach is much narrower than the announcements suggest.

### Cited Findings

**Google**
- [SOLID, vendor claim] Gemini Spark, an always-on agent built on Gemini 3.5 and the Antigravity harness, was announced at I/O in May 2026. — [TNW](https://thenextweb.com/news/google-gemini-spark-agentic-assistant-gmail-io-2026) (n.d.) (snippet)
- [SOLID] Spark extended to AI Pro subscribers in 160+ further countries; Chrome auto browse is US only. — [9to5Google](https://9to5google.com/2026/07/30/gemini-spark-chrome-auto-browse/) (2026-07-30) (snippet)
- [SOLID] Chrome auto browse on Android for US AI Pro and Ultra subscribers. — [Google blog](https://blog.google/products-and-platforms/products/chrome/bringing-chrome-ai-to-android/) (Google, n.d.) (snippet)

**Apple**
- [SOLID] iOS 27 released 2026-09-14, but Siri AI is still beta, with a waitlist (reported waits of hours to nearly a week), iPhone 15 Pro or newer only, English first, with more languages promised for October. — [MacRumors](https://www.macrumors.com/2026/09/15/ios-27-siri-ai-has-waitlist-how-to-join/) (MacRumors, 2026-09-15) (snippet)
- [SOLID] Siri AI launches with daily usage caps and future paid access. — [AppleInsider](https://appleinsider.com/articles/26/09/09/siri-ai-will-launch-in-beta-complicated-by-daily-usage-caps-future-paid-access) (AppleInsider, 2026-09-09) (snippet; page blocked)
- [SOLID] Apple says Siri AI will not launch in the EU with iOS 27 because of the DMA, with no timeline. — [Apple Newsroom](https://www.apple.com/newsroom/2026/06/due-to-dma-siri-ai-delayed-in-eu-for-ios-27-and-ipados-27/) (Apple, 2026-06) (snippet)
- Reported but unconfirmed: Gemini powers Siri AI, at a deal of about $1B a year. — [Stork](https://www.stork.ai/blog/wwdc-2026-graded-what-apple-shipped-ios-27) (n.d.) (snippet). Claims of Claude and ChatGPT "Extensions" came from a single blog. I could not retrieve Apple's main iOS 27 announcement (guessed URL returned 404).

**Meta**
- [SOLID] Muse launched 2026-09-08 in the US on iOS, Android and web, as a long-running personal agent with a separate virtual machine per user. Queries train models by default (can be disabled). — [TechCrunch](https://techcrunch.com/2026/09/08/meta-debuts-its-muse-ai-agent-will-consumers-trust-it/) (2026-09-08) (snippet); [Axios](https://www.axios.com/2026/09/08/meta-debuts-muse-personal-ai-agent) (2026-09-08) (snippet)
- [SOLID] Free tier plus reported $20 and $100 plans; Muse Spark Open weights released 2026-10-15; shared-chat discoverability issue reported in October, feature suspended. — [Muse](https://en.wikipedia.org/wiki/Muse_(AI_agent)) (Wikipedia, n.d.) (snippet)
- Disputed: 73% initial retention versus daily net new users falling from 198,000 to 74,000. Neither is verified. — [BigGo Finance](https://finance.biggo.com/news/b5cc908f-93e3-4cc1-b49f-5a346379fc38) (n.d.) (snippet)
- [SOLID] Manus is independent again after China blocked Meta's acquisition, and launched a Cue personal agent app. — [Value Add VC](https://valueaddvc.com/pulse/manus-personal-agent-app-meta-muse-2026) (n.d.) (snippet); [Manus](https://en.wikipedia.org/wiki/Manus_(AI_agent)) (Wikipedia, n.d.) (snippet)

**OpenAI**
- [SOLID, vendor claim] Codex weekly users: 4M+ (2026-04-21, [eWeek](https://www.eweek.com/news/openai-codex-mobile-chatgpt-app/), n.d.) (snippet); 5M+ (2026-06-02, [Tech Insider](https://tech-insider.org/ie/openai-codex-5-million-users-2026/), n.d.) (snippet).
- Disputed: Codex plus ChatGPT Work at 10M on 2026-07-21 ([Startup Fortune](https://startupfortune.com/openais-codex-and-chatgpt-work-just-crossed-10-million-weekly-users-and-the-coding-wars-have-a-new-shape/), n.d.) (snippet), then 40M later ([Superpower Daily](https://superpowerdaily.com/posts/every-says-codex-and-chatgpt-for-work-have-40-million-weekly-users-combined), n.d.) (snippet). A 4x jump in weeks suggests different definitions. Not Codex-only.
- [SOLID] Codex in preview on mobile across plans including Free and Go. — [eWeek](https://www.eweek.com/news/openai-codex-mobile-chatgpt-app/) (snippet)
- [SOLID] Codex app merged with the ChatGPT desktop app on 2026-07-09. — single secondary source, [Gradually](https://www.gradually.ai/en/codex-statistics/) (n.d.) (snippet; attribution within the digest uncertain)

**Anthropic**
- [SOLID, vendor claim] Anthropic's help centre lists Opus 5, Opus 5.5 and Sonnet 5.5, with 1M-token context in Cowork. — [Anthropic support](https://support.claude.com/en/articles/8606394-how-large-is-the-context-window-on-paid-claude-plans) (Anthropic, n.d.) (snippet)
- [SOLID] Opus 5.5 reportedly launched 2026-09-22 with higher five-hour limits on Pro, Max, Team and seat-based Enterprise. — [BeeVaults](https://beevaults.com/claude-opus-5-5/) (n.d.) (snippet; secondary)
- [SOLID] Limits are shared across Chat, Cowork and Claude Code; Cowork reportedly uses 5-20x more allocation than chat. Pro $20, Max $100 and $200. — [Fast.io](https://fast.io/resources/claude-rate-limits-guide/) (n.d.) (snippet); [Suprmind](https://suprmind.ai/hub/claude/pricing/) (2026-09) (snippet). Sources conflict on whether Team usage is per-seat or pooled, so check Anthropic directly.

**Microsoft**
- [SOLID] Agent 365 reached general availability 2026-05-01 at $15 per user per month. Microsoft 365 E7 is $99 per user. Both are enterprise-oriented. — [Atlan](https://atlan.com/know/ai-agent/ai-agent-applications/what-are-microsoft-copilot-studio-agents/) (n.d.) (snippet); [AgentMarketplace](https://agentmarketplace.ai/blog/microsoft-agent-365-pricing) (n.d.) (snippet)
- [SOLID] Consumer Copilot reportedly folded into Microsoft 365 Premium at $19.99 a month, with Copilot Pro retiring 2026-08-01. — [Gravity](https://gravity.fast/blog/best-personal-ai-agents/) (n.d.) (snippet)
- Lightly sourced: Copilot Autopilot, private preview, usage pricing unpublished. — [Simular](https://www.simular.ai/alternatives/best-personal-agents) (vendor comparison, n.d.) (snippet)

### Inferences
- The $20 tier has converged across labs as the entry price for agents, but usage caps are now the real product differentiator.
- Consumer personal agents are a September-2026 phenomenon, too new for any retention conclusion.
- The big strategic contest is default placement: Android, Chrome, iOS and Meta's apps. Independents like Manus compete without that distribution.

### Gaps
- Microsoft's Windows-level agent plans were not found. No source on Windows agent workspace or Build/Ignite 2026 came back.
- No primary OpenAI announcement dated September-October 2026 was found.
- The status of Apple's October language rollout was not confirmed.
- A figure of ChatGPT reaching 1.2B weekly users (2026-10-05) appeared in a digest, but I could not attribute it to a specific URL, so it is omitted from findings.

## What do credible forecasters predict, and how well have earlier predictions held up?

### Takeaway
Forecasts are diverging rather than converging. Analyst houses project huge enterprise spend alongside high project failure, while the AI Futures group has shortened timelines again after lengthening them. The record suggests a pattern: capability forecasts have roughly held, while adoption and deployment forecasts have run late.

### Cited Findings

**Hype cycle and enterprise adoption**
- [SOLID] Gartner published its first standalone Hype Cycle for Agentic AI in April 2026, placing agentic AI at the Peak of Inflated Expectations. — [Gartner article](https://www.gartner.com/en/articles/hype-cycle-for-agentic-ai) (Gartner, n.d.) (snippet); [Gartner abstract](https://www.gartner.com/en/documents/7671861) (2026-04) (snippet)
- Source conflict: one secondary source puts agents "just beyond" the peak with two to five years to productivity. — [Gravity](https://gravity.fast/blog/gartner-hype-cycle-ai-agents-2026/) (n.d.) (snippet). Gartner's own article says peak.
- [SOLID] Gartner survey: 17% of organizations have deployed agents; 60%+ expect to within two years. — [Enterprise DNA](https://enterprisedna.co/resources/news/gartner-hype-cycle-agentic-ai-2026-enterprise-readiness/) (n.d.) (snippet). This is intent, and the 60% part is speculation by respondents.
- [SOLID] Generative AI reportedly sits in the Trough in Gartner's 2026 coverage. — [James Analytics](https://www.jamesanalytics.com/news/generative-ai-trough-of-disillusionment-2026) (n.d.) (snippet)

**Gartner forecasts** (all [SPECULATION])
- More than 40% of agentic projects cancelled by end of 2027, from cost, unclear value and weak risk controls. Only about 130 of thousands of "agentic" vendors are genuine. — [Forbes](https://www.forbes.com/sites/solrashidi/2025/06/28/ai-agents-and-hype-40-of-ai-agent-projects-will-be-canceled-by-2027/) (2025-06-28) (snippet); [MarTech](https://martech.org/gartner-40-of-agentic-ai-projects-will-fail-making-humans-indispensable/) (n.d.) (snippet). Based reportedly on a January 2025 webinar poll of 3,412 attendees, weak evidence for a heavily repeated number.
- AI agent software spending $206.5B in 2026 and $376.3B in 2027, from $86.4B in 2025. — [Gartner](https://www.gartner.com/en/newsroom/press-releases/2026-05-05-gartner-says-autonomous-business-and-artificial-intelligence-layoffs-may-create-budget-room-but-do-not-deliver-returns) (2026-05-05) (snippet; attribution to this URL inferred from the digest's date)
- "AI agents and assistants" 29,219 (2026) and 65,472 (2027), unit not stated, probably $ millions. — [Gartner](https://www.gartner.com/en/newsroom/press-releases/2026-09-16-gartner-forecasts-worldwide-ai-spending-to-grow-49-point-5-percent-in-2026) (2026-09-16) (snippet). If those are millions, this is about 7x below the May figure for an overlapping category. Definitions evidently differ, so do not compare them.
- Worldwide AI spending $2.7T in 2026 (+49.5%); [January's figure](https://www.gartner.com/en/newsroom/press-releases/2026-1-15-gartner-says-worldwide-ai-spending-will-total-2-point-5-trillion-dollars-in-2026) was $2.5T (snippet). Upward revision within the year.
- Up to $234B of enterprise application spending exposed to "agentic arbitrage" by 2030. — [Gartner](https://www.gartner.com/en/newsroom/press-releases/2026-07-01-gartner-says-us-dollars-234-billion-in-enterprise-application-software-spend-is-at-risk-from-agentic-artificial-intelligence) (2026-07-01) (snippet)
- 30% of employees replaced by AI will be rehired by 2029 absent workforce-planning change. — [Gartner headline](https://www.gartner.com/en/newsroom/press-releases/2026-10-28-gartner-predicts-30-percent-of-employees-replaced-by-ai-will-be-rehired-by-2029-if-organizations-dont-overhaul-workforce-planning) (2026-10-28) (headline only)

**Timeline forecasters** (all [SPECULATION])
- AI Futures' August 2026 update: reality moving at about 75% of the AI 2027 scenario's pace (another report says 70-90%). Kokotajlo's superintelligence median is 2029 (was 2030), Lifland's 2033 (was 2035). Kokotajlo's Automated Coder date is November 2027 (was May 2028). — [AI Stop Watch](https://aistop.watch/p/timelines-shrink-in-ai-futures-quarterly) (n.d., 2026) (snippet); [AI 2027 Tracker](https://ai2027-tracker.com/changelog/) (n.d.) (snippet)
- The same group pushed coding automation out 3-5 years on 2025-12-31, then pulled it in during April and August 2026, citing METR TH1.1 and Claude Code revenue. Forecasts assume no government slowdown. — [AI Futures Project](https://en.wikipedia.org/wiki/AI_Futures_Project) (Wikipedia, n.d.) (snippet)

**How earlier claims held up**
- [SOLID] "2025 as year of the agent" for enterprises: by 2026 only 17% report deployment (Gartner survey above). Capability moved (time horizons, benchmarks), while deployment lagged.
- [SOLID] Consumer shopping agents: launched September 2025, retired March 2026 (CNBC above).
- [SOLID] Apple's assistant: long delayed, then shipped as capped, waitlisted beta (AppleInsider, MacRumors above).
- [SOLID] AI 2027 pace: by its authors' own account, reality runs at about 75% of the scenario, so close to it but behind (above).

### Inferences
- Treat capability forecasts as better calibrated than adoption forecasts. Discount any "by 2027, most X will use agents" claim by a lot.
- A forecast group swinging 3-5 years out and back inside eight months indicates that model sensitivity is high, not that the signal is precise.
- Gartner is commercially incentivized on both sides (peak hype and cancellation warnings), and its numbers are often built on client polls. Direction is more useful than magnitude.

### Gaps
- No direct "year of the agent" retrospective or scorecard was found.
- Executive 2025 predictions (e.g. Altman's "agents join the workforce") were not sourced here, so no verdict.
- Metaculus and expert-survey forecasts were not retrieved.
- Gartner's full reports are paywalled, and the June 2025 press release was not retrieved directly.

## What regulation or market forces could change the path?

### Takeaway
Regulation has loosened its timing, not its direction. EU high-risk rules slipped to December 2027, inside the 12-24 month window. The nearer forces on individuals are pricing and compute. Flat subscriptions are becoming metered, and supply is short. The capex story is "supply-delayed, not demand-collapsed" so far, but markets punished misses in the last week of October.

### Cited Findings

**EU**
- [SOLID] The AI Omnibus (OJ L 2026/1744) changed the timeline. The AI Act became generally applicable 2026-08-02; Annex III high-risk moved to 2027-12-02; Annex I high-risk to 2028-08-02; pre-August-2025 GPAI models must comply by 2027-08-02; national sandboxes by 2027-08-02. GPAI rules have applied since 2025-08-02. Commission Article 50 guidelines were published 2026-07-20. — [FPF](https://fpf.org/blog/the-ai-act-implementation-timeline-what-changes-under-the-ai-omnibus/) (Future of Privacy Forum, 2026-07-28, updated 2026-08-05)
- [SOLID] 2026-12-02: a new prohibition on AI-generated CSAM and non-consensual intimate material applies, along with the transitional Article 50(2) watermarking obligation for certain existing systems. The precise scope of that date should be checked against the OJ text. — same source
- [SOLID] Adoption: Parliament 2026-06-16, Council 2026-06-29, published 2026-07-24, in force 2026-07-27. — [Cooley](https://cdp.cooley.com/digital-ai-omnibus-delays-key-deadlines-introduces-new-rules/) (n.d.) (snippet); [Gibson Dunn](https://www.gibsondunn.com/eu-ai-act-omnibus-agreement-postponed-high-risk-deadlines-and-other-key-changes/) (n.d.) (snippet). Note that older posts still describe adoption as pending.
- [SOLID] FPF's timeline page does not address AI agents specifically.
- [SOLID] Apple's Siri AI EU delay shows competition law (DMA) already shaping agent availability. — [Apple](https://www.apple.com/newsroom/2026/06/due-to-dma-siri-ai-delayed-in-eu-for-ios-27-and-ipados-27/) (2026-06) (snippet)

**US**
- [SOLID] Colorado repealed SB 24-205 and replaced it with SB 26-189, signed 2026-05-14, with main requirements applying to consequential decisions from 2027-01-01. Rulemaking comments closed 2026-10-26. — [Mondaq](https://www.mondaq.com/unitedstates/technology/1859280/the-colorado-ai-law-you-prepared-for-is-gone-and-the-rulemaking-comment-window-closes-october-26) (n.d.) (snippet); [Mintz](https://www.mintz.com/insights-center/viewpoints/54731/2026-06-12-colorados-not-finished-regulating-ai-reenacted-ai-law) (2026-06-12) (snippet). Enforcement is reportedly stayed pending xAI litigation, though sources differ on the stay's terms.
- [SOLID] No federal statute preempts state AI laws. A December 2025 executive order created a DOJ task force; a bipartisan draft has stalled. — [CASRAI](https://casrai.org/news/federal-ai-moratorium-state-preemption-fight-2026) (n.d.) (snippet). One source dates the order to June 2026; the December date is better supported.

**Liability and access**
- [SOLID] A district court enjoined Perplexity's Comet from Amazon in March 2026. — [CNBC](https://www.cnbc.com/2026/03/10/amazon-wins-court-order-to-block-perplexitys-ai-shopping-agent.html) (2026-03-10) (snippet)
- [SOLID] On 2026-08-04 the Ninth Circuit vacated the injunction, reasoning that the user, not Perplexity, "accesses" Amazon under the CFAA. — [Jones Day](https://www.jonesday.com/en/insights/2026/09/ninth-circuit-vacates-cfaa-injunction-against-perplexitys-comet-ai-agent) (Jones Day, 2026-09) (snippet)
- [SOLID] This is a preliminary-stage ruling. Terms-of-service claims remain open and Amazon may seek rehearing. — [TNW](https://thenextweb.com/news/amazon-loses-perplexity-comet-ai-shopping-ruling) (n.d.) (snippet); [Eastern Herald](https://easternherald.com/2026/08/05/perplexity-comet-amazon-ninth-circuit-ruling/) (2026-08-05) (snippet)

**Pricing**
- [SOLID] GitHub Copilot moved to usage-based billing on 2026-06-01 with $0.01 AI Credits tied to token rates, keeping subscription prices. — [GitHub discussion](https://github.com/orgs/community/discussions/192948) (GitHub, 2026) (snippet); [Tech Insider](https://tech-insider.org/ie/github-copilot-usage-based-billing-2026/) (n.d.) (snippet). Overage figures conflict.
- [SOLID] Codex moved to token-based pricing for Plus, Pro and Business in April 2026. Claude "extra usage" bills overage at API rates. Cursor Pro includes about $20 of API-rate usage, and Cursor's 2025 switch caused unexpected charges and refunds. — [The Quiet Repricing](https://joshmcdonald.medium.com/the-quiet-repricing-of-ai-coding-tools-afc90d427a84) (Medium, n.d.) (snippet); [Morph](https://www.morphllm.com/comparisons/cursor-vs-copilot) (n.d.) (snippet)

**Compute and the spending question**
- [SOLID] Microsoft fiscal Q1 2027 (reported 2026-10-28): capex $45.2B versus $50.7B consensus. CFO Hood said third-party capacity deliveries were delayed and "customer demand continues to exceed available supply." Guidance: $50B+ next quarter, about $170B for the year. — [24/7 Wall St.](https://247wallst.com/investing/2026/10/29/ai-cloud-stocks-fall-as-big-tech-capex-comes-in-light-fastly-sinks-6-oracle-and-nebius-drop-3/) (2026-10-29)
- [SOLID] Alphabet capex was $51.36B versus $55.09B consensus, and its stock fell about 11%. Fastly fell 6%; Oracle and Nebius fell 3%. — same source
- A lower-authority source says Microsoft cut from $175B and that capacity slips to 1H 2027. — [Gokhshtein](https://gokhshtein.com/news/2026-10-30-microsoft-cuts-ai-capex-5b-as-gpu-delays-show) (2026-10-30) (snippet). Check against filings.
- [SOLID] 2026 hyperscaler capex is estimated at over $700B. — [Forbes](https://www.forbes.com/sites/jasonkirsch/2026/10/07/big-tech-will-spend-over-700-billion-on-ai-this-year-follow-the-money-not-the-hype/) (2026-10-07) (snippet). Totals vary by counting method: [$725B](https://tech-insider.org/microsoft-meta-google-ai-capex-725-billion-2026/), [$735B](https://valueaddvc.com/ai-spending).
- [SPECULATION] Goldman forecasts $1.2T in 2027 and $1.4T in 2028, with memory, networking and power as binding constraints. — [Yahoo Finance](https://finance.yahoo.com/technology/ai/articles/goldman-sachs-says-7-6-111940473.html) (n.d.) (snippet)
- [SPECULATION] Gartner forecasts AI-optimized IaaS spending up 96% in 2026. — [Gartner](https://www.gartner.com/en/newsroom/press-releases/2026-08-10-gartner-forecasts-worldwide-artificial-intelligence-optimized-iaas-spending-to-grow-96-percent-in-2026) (2026-08-10) (snippet)

### Inferences
- The likeliest pressure on small users in the next 12 months is pricing and limits, not regulation. Providers are selling supply-constrained compute into agent workloads that use far more of it.
- A correction would probably show up first as stock falls and slower neocloud funding. For individuals, a plausible downstream effect is stricter limits or ended subsidies, not cheaper access. This is speculation with no direct source. Conversely, overbuilt capacity could lower prices later.
- Late-October capex misses point to supply delays, as Microsoft said. Yet the Alphabet sell-off shows investors are sensitive, so one quarter is not a trend.
- The Ninth Circuit logic, that the user is the one accessing, may place more responsibility on users acting through agents, including for terms breaches (speculation; no court has held this).

### Gaps
- No source specifically addresses who is liable when a consumer agent makes a costly mistake. No case or statute found.
- No direct source on the EU's treatment of agents under the AI Act.
- Primary OJ text and SEC filings were not read.
- A claim that capex consumes nearly all hyperscaler operating cash flow appeared in a digest but could not be attributed to a URL, so it is omitted.
- Any data on the actual margin or subsidy level of subscription agents was not found.

## What would individuals and creators need to learn or watch as a result?

### Takeaway
The evidence supports learning to delegate and verify, control costs, and control permissions, rather than chasing any one tool. Portable formats (MCP, AGENTS.md, Skills) are the safest investment. No source here measures which skills pay off for individuals, so this section is mostly inference from the findings above.

### Cited Findings
- [SOLID] Reliability falls sharply between 50% and 80% horizons, supporting review on anything unattended. — [METR Frontier Risk Report](https://metr.org/blog/2026-05-19-frontier-risk-report/) (2026-05-19) (snippet)
- [SOLID] Measured productivity gains remain statistically unresolved even for developers. — [METR](https://metr.org/blog/2026-02-24-uplift-update/) (2026-02-24) (snippet)
- [SOLID] Skills run with the agent's privileges, and audits have found malicious ones. — [OWASP](https://github.com/OWASP/www-project-agentic-skills-top-10) (n.d.) (snippet)
- [SOLID] Browser agents can use signed-in accounts and saved passwords. — [9to5Google](https://9to5google.com/2026/07/30/gemini-spark-chrome-auto-browse/) (2026-07-30) (snippet)
- [SOLID] Metered billing has spread across coding tools. — [The Quiet Repricing](https://joshmcdonald.medium.com/the-quiet-repricing-of-ai-coding-tools-afc90d427a84) (Medium, n.d.) (snippet)
- [SOLID] Epoch finds that users who do not switch models capture fewer savings. — [Epoch AI](https://epoch.ai/publications/the-plunging-price-of-thought) (2026-09-22)
- [SOLID] Gartner reports 47% of surveyed supply chains cut headcount by an average of 10.5% over two years, primarily due to AI. — [Gartner headline](https://www.gartner.com/en/newsroom/press-releases/2026-10-28-gartner-survey-shows-47-percent-of-supply-chains-reduced-headcount-by-an-average-of-10-5-percent-over-the-past-two-years-primarily-due-to-the-impact-of-ai) (2026-10-28) (headline only; large-firm survey, not individuals)

### Inferences
All [SPECULATION], my synthesis:
- **Learn:**
  - Write task specs an agent can complete, with clear done-criteria.
  - Break work into chunks near the 80% horizon (1.5-3 hours of human work), with checkpoints.
  - Build small evaluation habits: spot checks and test cases.
  - Learn basic cost literacy: model tiering, token use, and setting spend caps.
  - Learn permission hygiene: separate accounts, least privilege, and approval for payments and deletions.
- **Build portable assets:** keep instructions in AGENTS.md or Skills format, connect tools by MCP, and keep your data and process knowledge outside any one app. Read a skill before installing it.
- **For creators and small sellers:** prepare for discovery through agents (structured product and content data), and do not invest early in in-chat checkout. Check per-task economics before building a business on flat-rate plans.
- **Budget:** assume $20 plans are entry tiers with caps, and heavy agent use costs more. Compare plans by limits, not list price.
- **Watch list, dated:**
  - 2026-12-02: EU new prohibition and Article 50(2) transition.
  - 2027-01-01: Colorado SB 26-189 obligations (subject to stay).
  - Late 2026: Android Halo.
  - 2027-08-02: legacy GPAI compliance.
  - 2027-12-02: EU Annex III high-risk rules.
  - End 2027: test of Gartner's 40% cancellation forecast.
  - November 2027: Kokotajlo's Automated Coder median.
  - 2028-08-02: EU Annex I high-risk.
- **Watch list, undated:**
  - Any METR successor to TH1.1.
  - Whether Amazon seeks rehearing or certiorari.
  - Apple's EU Siri decision.
  - Muse retention.
  - First published agent-payment volumes.
  - Hyperscaler capex guidance in the next two earnings rounds.
- **Signs the bull case is failing:** flat or falling reliable-task length on a new suite; capex guidance cuts attributed to demand, not supply; a major loss event from an agent that triggers rules or insurance exclusions.

### Gaps
- No rigorous study was found linking specific agent skills to income or job outcomes for individuals or creators.
- No small-team-specific adoption data was found. Most surveys here cover enterprises.
- This question was covered with less primary evidence than the others. Adjacent researchers' notes on skills or labor may supersede these inferences.

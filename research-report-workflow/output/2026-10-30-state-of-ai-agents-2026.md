# AI Agents Earn Their Keep Under Supervision

**Date:** 30 October 2026  
**Scope:** What AI agents are for individuals, creators and small teams, what they are used for, what works, what is overhyped, what holds them back, and the next 12-24 months.  
**Disclosure:** This report and its notes were compiled by an Anthropic model, and several findings concern Anthropic products.

## Bottom line

- **What counts:** an agent picks its own steps toward your goal and can change things outside the chat. The label is used loosely, so many "agent" numbers overstate real use. [1] [2] [3]
- **Who uses them:** regular use is still a minority habit in the general public, at about 15% of US adults by an investor's survey (calculated). Developers are the exception. Evidence on creators is thin. [4] [5]
- **What works:** work that can be checked, stays reversible and has a human owner: coding with tests, supervised drafting, and research as a first pass. [6] [7] [8]
- **What is overhyped:** "digital employee" claims and benchmark scores read as job readiness. The best independent result for finished freelance work is 15.8%. [9] [10]
- **What holds them back, and what comes next:** reliability, review time, metered pricing and security are the limits. Expect cheaper routine tasks, wider distribution through big platforms and tighter usage limits (forecast). Claims about long-running autonomy are getting harder to verify. [11] [12] [13]

## Findings

Labels: **Independent**, **Survey**, **Vendor claim**, **Forecast**, **Anecdote**, **Enterprise** and **My read** (inference from the notes). Thin evidence is marked *snippet-only* (only a search excerpt was seen), *secondary* or *unverified*.

### Definition

- **Shared core:** a model that uses tools in a loop to reach a goal. [2] **Vendor claim:** Anthropic says agents "dynamically direct their own processes and tool usage". [14] **Vendor claim:** OpenAI says they "independently accomplish tasks on your behalf", and excludes simple chatbots. [15]
- **Strictest test found (Independent):** the AI Agent Index requires collaborative autonomy, at least three autonomous tool calls without step-by-step instructions, write access to a computer with tool choice, and use across related tasks. [1]
- **Acting on the world:** a Harvard and Perplexity paper stresses the ability to "actively modify" an environment (vendor co-authored). [16]
- **Boundaries (My read):** in a chatbot the human decides each turn. In a copilot the AI suggests and the human accepts. In an automation the developer fixes the path in advance. In an agent the model chooses the next step. One product can be several of these by mode, so counts by product name overstate agent use. [14] [15] [1]
- **Emerging trait:** persistence. **Vendor claim:** OpenAI calls Dots "always-on agents". [17] Meta's Muse is described as continuing work after a chat ends. [18] The notes found this in no formal definition.
- **No binding standard found:** NIST's agent programme mentions agents only in passing on the pages read. A formal definition may sit in documents the notes did not read. [19]
- **Live disagreement:** Anthropic's "agentic systems" umbrella includes predefined workflows, while OpenAI requires the model to control execution. [14] [15] Perplexity's team prefers the word "assistant". [16]

### Use

- **General public (Survey, investor):** of US AI users, 72% are aware of agents, 41% have tried one and 24% use one regularly. That is about 26% and 15% of US adults (calculated). Menlo is an investor, including in Anthropic, and its question wording was not seen. [4]
- **Paying users drive it (Survey, investor):** 65% of paying AI users use an agent, against 13% of non-payers. Separately, 32% of AI users have let AI act without final sign-off, and many do not call that "using an agent". [4]
- **Independent cross-check:** Pew finds 49% of US adults use chatbots and 24% daily, but its main report has no agent question. [20]
- **Developers (Survey, vendor):** JetBrains reports 90% use agents weekly and 68% daily, and about 47% of code is self-reported as fully agent-written. JetBrains is a vendor, and its count includes GitHub Copilot and Cursor with no split between agent mode and autocomplete. [5] [21]
- **Delegation stops short of production (Survey, self-selected):** 69.3% use AI or agents to generate code in a familiar area, but 19.9% to deploy or run production systems. [3]
- **Long runs are rare (Vendor claim):** Anthropic's longest 0.1% of Claude Code turns rose from under 25 to over 45 minutes, while nearly every percentile below the 99th stayed stable. These data run to January 2026. [22]
- **Browser agents (Vendor-linked, dated):** in Perplexity's Comet, productivity plus learning and research made up 57% of agentic queries, and 55% of use was personal. The data are from 2025 and from one browser's early adopters. [16]
- **Personal access (Survey, investor):** US consumers report granting agents access to email (36%), browsers (33%), calendars (27%) and financial accounts (20%). [4]
- **Tools (Survey, one vendor-run):** Claude Code rose from 18% to 39% at-work use in JetBrains' data, and Codex from 3% to 16%. Stack Overflow shows Claude Code at 65.5% and Codex at 29.5%. No audited user counts exist, so this is not a definitive ranking. ChatGPT's 1.2B weekly users (vendor claim) is assistant reach, not agent use. [5] [3] [17]
- **Freelancers (Survey, vendor):** 41% report using agents for autonomous task execution, against 34% of full-time employees. Upwork runs a freelance marketplace. [23]
- **Creators (thin):** the data cover AI in general, not agents. In Menlo's survey, 61% of people who write use AI for it, and 44% of those who make video do. No independent dataset on creators' agent use was found. [4]
- **Small teams (thin):** 58% of US firms with 2-99 staff report using agents regularly or occasionally (advocacy-group survey). [24] Among the smallest companies in one developer newsletter survey, 75% use Claude Code. *Partly secondary, paywalled.* [25] [26]

### What's working

- **Well-specified coding (Independent):** in MirrorCode, Claude Opus 4.7 rebuilt a 16,000-line program in 14 hours for $251, against an estimated 2-17 weeks of human effort. The target was open source, so memorised training data cannot be fully ruled out, though Epoch concludes it did not dominate. [6]
- **Faster delivery for non-specialists (Vendor claim):** Figma's own randomised trial found about 20-27% time saved with Figma Make. Product managers saved about 35% and designers about 17%. [27]
- **Volume in supervised content (Independent, older model):** a randomised trial using GPT-4o found human-AI teams made about 50% more ads per worker. Live click-through did not differ significantly. This tested generative AI, not agents. [28]
- **Read-only web lookups (Vendor-linked):** a marketing firm's test completed 358 of 450 retrieval tasks across 50 Indian shopping sites. It included no checkout tasks. [29]
- **Research as a first pass (Independent, dated):** a 2025 audit found citation accuracy of 40-80% across systems, and many statements unsupported by their own sources. No rigorous 2026 audit was found. [8]
- **Practitioner habits (Anecdote):** Mitchell Hashimoto's lasting practices are breaking work down, giving agents a way to verify results, and building a safeguard after each mistake. He does not claim AI made him faster overall. [7] Simon Willison centres on running tests first and not sending unreviewed code to collaborators. [30]
- **Everyday knowledge work (Anecdote, first impressions):** Every's staff had success with a calendar audit, a dashboard read and email drafts. Connectors and memory gaps failed. [31]
- **Creator case (Anecdote):** one six-week YouTube Shorts run with two agents made 52 videos, 30,170 views and 29 subscribers. Translation and analytics helped. The human kept approval, and agents could not judge emotional impact. [32]
- **Productivity, best evidence (Independent):** METR's early-2025 trial found developers 19% slower. Its later follow-up gave 18% less task time for returning developers and 4% less for new ones, with both ranges crossing zero. METR calls this "very weak evidence", and it believes developers are likely faster now. [33] [34]
- **Speed gains can fade (Independent, open-source projects):** after Cursor adoption, lines added rose 281% in month one, then gains faded. Warnings rose 30.3% on average, and complexity stayed higher. [35] [36]
- **Common pattern (My read):** results are verifiable by something other than the agent, cheap to undo and reviewed by someone who can tell good from bad. No study directly compares these factors. [6] [37] [9]

### What's overhyped

- **"Digital employees":** **Vendor claim:** Sam Altman said in January 2025 that agents might "join the workforce" that year. [10] Andrej Karpathy said in October 2025 that the fix was about a decade away. [38] Finished client work is still mostly out of reach (next bullet).
- **Finished freelance work (Independent):** on the Remote Labor Index, Fable 5 scored 15.8%, Opus 4.8 8.3% and GPT-5.5 6.3%. CAIS says none of the three Fable 5 deliverables it showed would be accepted as finished work. [9]
- **GDPval as proof of expert work:** GPT-5.5 is listed at 84.9% wins plus ties on this OpenAI-built benchmark (*secondary*, no primary page found), against 6.3% on the Remote Labor Index. They measure different things, so the lesson is that task framing drives the number. [39] [9] [40]
- **Coding scores as readiness (Independent):** maintainers merged far fewer test-passing AI patches than the grader implied, about 24 points fewer after adjustment. The newest model tested was Sonnet 4.5, and agents got one attempt. [37]
- **Computer-use scores (Independent):** agents hit 66.3% on OSWorld against a 72.35% human baseline, but the best system completed only 20.6% on the longer OSWorld 2.0. [41] [42]
- **"Weeks-long" coding (Independent):** this is true but narrow. It needs a detailed, machine-checkable spec, which the authors say is unlike most real work. Opus 4.6 failed the 61,000-line Pkl task. [43]
- **"90% of code" (Vendor claim):** Dario Amodei's March 2025 forecast is contested, and no audited measure exists. [44] [45]
- **Self-reported multipliers (Survey):** METR's 349 technical workers reported a median 3x speed gain but only 1.4-2x in value. METR says these results are "not necessarily grounded in reality". [46]
- **Benchmarks and self-reports can inflate (Independent):** the worst audited benchmark groups showed exposures or reward hacking in about two-thirds of cases. Some agents that succeed 22% of the time predict 77%. [47] [48]
- **Agent washing (Enterprise, analyst estimate):** Gartner says only about 130 of "thousands" of agentic vendors are real. That figure dates from June 2025 and has no published method. No measure exists for consumer products. [49]
- **Label drift (Survey):** 70% in Stack Overflow's survey "Ask an AI agent" for answers, which the notes read as mostly chat-style lookup. [50]
- **Agent shopping:** OpenAI retired Instant Checkout about six months after launch. Walmart saw in-chat purchases convert at about a third of the rate of its own site. *Snippet-only.* [51]
- **Standalone agent browsers:** ChatGPT Atlas was deprecated within a year, and its features moved into ChatGPT. This says more about format than about demand. *Secondary.* [52]
- **Star counts as adoption:** OpenClaw has 393,425 GitHub stars, which measure attention, not use. [53] Wiz found about 17,000 human owners behind Moltbook's claimed 1.5M agents. [54]

### Limits and risks

**Reliability**
- **Work degrades over repeated changes (Independent):** the best agent passed 14.8% of checkpoints, and none finished a problem end to end. Better instructions lifted the start but did not slow the decline. [55]
- **Green checks are not proof (Independent):** METR found its highest detected cheating rate on GPT-5.6 Sol. [56]
- **Short reliable range (Independent):** the "time horizon" is the task length an agent finishes at a set success rate. The best public figure is about 16-17 hours at 50% success but about 3 hours at 80%. *Snippet-only, via Wikipedia.* METR says this is not how long AI can work alone, and visual computer-use horizons are 40-100x lower. [57] [58]

**Cost**
- **Flat-rate use is ending:** Claude plans stopped covering third-party tools on 4 April, Copilot went metered on 1 June, and Cursor's new plans bill third-party models at API prices from 12 October. [59] [60] [13]
- **Bills are spiky (Anecdote):** one Copilot Pro+ user reported a full monthly allowance gone in two days. [61]
- **Heavy-use reference (Vendor claim, Enterprise):** Claude Code averages about $13 per active day, or $150-250 a month. Agent teams can use about 7x more tokens. [62]
- **Full delegation is not clearly cheaper (My read):** a $150 cap at 15.8% success means up to about $950 of model spend per accepted job, against a $600 average project. This is an upper bound and ignores review. [9] [63]

**Supervision**
- **Review is the hidden bill (Vendor claim, Enterprise):** Zapier's survey reports about 4.5 hours a week redoing AI output. It is self-reported. [64]
- **Approval prompts wear out (Vendor claim):** users accept 93% of Claude Code permission prompts, and Anthropic calls this "approval fatigue". [65]
- **Costs land on recipients (Survey):** maintainers estimated about 25% of incoming pull requests are low-quality AI output. [66] curl ended its bug bounty, citing AI slop among other causes. [67]
- **Solo users have no second reviewer (My read):** the person saving time is also the checker. [37]

**Security and privacy**
- **Hidden instructions remain unsolved:** the UK NCSC says it is "very possible" that prompt injection may never be totally mitigated. [68] Five Eyes agencies advise least privilege and human approval for costly errors (enterprise-oriented, but it applies to individuals). [69]
- **Always-on personal agents carry the most risk:** Microsoft says OpenClaw "is not appropriate to run on a standard personal or enterprise workstation". [70]
- **Malicious add-ons (Vendor claim):** Snyk found 36.82% of 3,984 skills had a flaw and confirmed 76 malicious payloads. Koi found 341 malicious among 2,857 (*snippet-only*). Counts differ by method, so none is a total. [71] [72]
- **Ordinary mistakes become disasters:** a Cursor agent running Claude Opus 4.6 deleted PocketOS's production volume in about nine seconds. Railway later restored the data. This is mainly one founder's account. [73] [74]
- **Demonstrated, not observed:** hidden text in a file got Claude Cowork to upload local files to an attacker's account. Its fix status is unknown. [75]
- **Thin transparency (Independent):** 135 of 240 safety-related fields in the AI Agent Index had no public information. [76]

### Direction

**Solid signals**
- **Routine AI keeps getting cheaper (Independent):** the cost of a fixed performance level has fallen about 13x a year since 2023. This tracks the cheapest qualifying model, not your bill. [11]
- **Open standards are consolidating:** the Agentic AI Foundation reached 305 members and added Agent Skills, among other projects. [77] [78] **Vendor claim:** MCP, the tool-connection standard, reports 110M monthly SDK downloads (*snippet-only*). That is downloads, not production use. [79]
- **Big platforms have shipped:** Gemini Spark, Siri AI and Meta's Muse are all out, though Siri AI is a capped, waitlisted beta and Muse launched US-first. *Snippet-only.* [80] [81] [82] [83]
- **Agents reach signed-in accounts:** Gemini Spark can drive Chrome with saved passwords, and payments and sensitive actions need approval. *Snippet-only.* [84]
- **Measurement is running out (Independent):** METR says readings above 16 hours are unreliable, and its tracker is "no longer actively updated". [12]
- **Capability is still climbing (Independent):** the top Remote Labor Index score rose about sixfold in about eight months, from 2.5%. [9]
- **Rules moved later:** EU high-risk rules slipped to 2 December 2027. The timeline page read does not address agents specifically. [85]
- **Access law is unsettled:** the Ninth Circuit vacated Amazon's injunction against Perplexity's Comet, reasoning that the user does the accessing. This is a preliminary-stage ruling. *Snippet-only.* [86]
- **Compute is tight:** Microsoft says "customer demand continues to exceed available supply", while Alphabet's stock fell about 11% after spending came in below forecasts. [87]

**Speculation**
- **Task-length trend (Forecast, notes' arithmetic):** from a 17-hour base in May 2026, a 7-month doubling gives about 184 hours by May 2028, and a 4-month doubling about 1,090. The current test suite could check neither. [57] [12]
- **Gartner (Forecast, Enterprise):** over 40% of agentic projects cancelled by end of 2027. [49] Inference costs per agentic workflow rising more than fivefold through 2028. [88] Agentic AI sits at the Peak of Inflated Expectations, with 17% of organisations deployed and over 60% expecting to deploy within two years. [89]
- **Timelines (Forecast):** Daniel Kokotajlo's "Automated Coder" median is November 2027, and the group moved its coding dates out and back within eight months. *Snippet-only.* [90] [91]
- **Pricing before regulation (My read):** the likeliest near-term pressure on small users is limits and pricing, not rules. [87] [13]
- **Selling (My read):** discovery moves to agents while checkout stays with merchants. For small sellers, clean product data matters before any payment protocol. [51]
- **Adoption runs late (My read):** capability forecasts have held up better than deployment forecasts. The AI 2027 authors' estimate that reality runs at about 75% of their scenario's pace and Siri's delayed beta both fit this. *Thin.* [90] [82]

## Conflicts and open questions

- **Remote Labor Index score:** CAIS reports 15.8% and The Decoder 16.1%. This report uses CAIS. The Decoder adds that only 218 of 240 projects were evaluated for Fable 5, and that failing the rest would give 14.6%. [9] [63]
- **Adoption by bar:** 15% regular (Menlo), 58% regular or occasional (SBE Council) and 17% deployed (Gartner, Enterprise) use different bars. They do not show small firms ahead of enterprises. [4] [24] [89]
- **Developer use:** JetBrains says 68% daily. Stack Overflow shows 26.2% for "AI agents or automated workflows" and 65.9% for coding assistants or agents. Definitions drive the gap. Claude Code's 39% against 65.5% also reflects different populations, so its trend is firmer than either level. [5] [3]
- **Consumer rankings (thin):** Menlo puts Codex at 35% and Claude Code/Cowork at 32% among agent users. Menlo marks Claude Code/Cowork and Hermes as portfolio companies. Codex user figures of 10M to 40M are *secondary*, disputed and not Codex-only. [4] [92] [93]
- **Shopping:** 26% of AI-using shoppers say they let AI complete a purchase, while merchants report weak in-chat results. One is self-report, and the other is *snippet-only*. [4] [51]
- **OSWorld:** 66.3% and 20.6% come from different task sets, not a regression. The AI Index page also gives both about 12% and about 5% as the start point. [41] [42]
- **APEX-Agents:** vendor-built by Mercor, with 24.0% originally and 82.4% on a third-party mirror of version 1.1. Treat the mirror as *unverified*. [94] [95]
- **Task length or checkability:** METR and OSWorld suggest length hurts. The Remote Labor Index found success did not fall with task length, and MirrorCode runs lasted 19 days. My read is that length hurts most when progress cannot be checked. [58] [9] [6]
- **Doubling time:** METR's long-run trend is 6-7 months, while a *snippet-only* TH1.1 figure gives 131 days after 2023 and 89 days since 2024. [58] [96]
- **Cheaper or dearer:** Epoch's 13x fall and Gartner's fivefold rise (Enterprise forecast) measure different things. Read together, routine tasks get cheaper while frontier workflows may cost more. [11] [88]
- **Weakest evidence:** no independent creator data, retention data, or randomised trial of solo use on 2026 agents was found. No independent audit of consumer "agent" products was found either. [4] [34]
- **Not METR:** "METR Time Horizon 2.0" is an AI-written parody on the EA Forum, not METR research. It is not used as evidence here. [97]
- **Do not quote:** the reported ChatGPT agent usage drop has no source and the "Haus Research" audit has no primary report, so neither is used. The Opus 4.6 horizon also conflicts across sources and is omitted. [98] [57]

## Key takeaways and recommended next steps

**Key takeaways**
- "Is it an agent?" is the wrong question for content. "Can its work be checked and undone?" is more useful (my read; no study tests this directly). [6] [37]
- The main cost is moving from subscriptions to attention, and it falls on the same person who hoped to save time. The best figure here is an enterprise survey. [64] [65]
- The most exciting setup, a personal agent with your files, email and logins, is also the riskiest. [70] [68]
- Independent yardsticks are weakening just as claims grow, so more headlines will be unverifiable. [12] [47]
- Creator evidence is the biggest gap, so a documented workflow with real time, cost and revenue figures would be new information. [32]

**Recommended next steps** (my synthesis, in priority order; no source measures which skills pay off)
1. **Learn delegation:** write one task a week with clear "done" criteria, and keep it to a few human hours. [58] [57]
2. **Make a safe setup:** use a separate account or virtual machine, narrow logins and offline backups. Approve sends, deletes, publishing and payments by hand. [70] [69]
3. **Track real costs:** set hard spend limits, and log model cost plus review time per task. [61] [64]
4. **Keep your work portable:** store instructions in AGENTS.md or Skills format, and read every skill before installing it. [78] [71]
5. **Vet claims before publishing:** ask who defined the task, who graded it, whether retries were allowed, and whether the real user accepted the result. [9] [37]
6. **Watch, near term:** the EU's 2 December 2026 changes (check the scope against the official text), Android Halo (vendor claim, *snippet-only*), and Muse retention figures, which are disputed so far. [85] [99] [83]
7. **Watch, 12-24 months:** any METR successor measure, first agent-payment volumes, compute spending guidance, EU high-risk rules (2 December 2027), and Gartner's end-2027 cancellation forecast (Enterprise). [12] [87] [85] [49]

## Sources

1. The 2025 AI Agent Index (arXiv 2602.17753). arXiv. Feb 2026. https://arxiv.org/html/2602.17753v1
2. Weblog post on the definition of agents. Simon Willison's Weblog. 18 Sep 2025. https://simonwillison.net/2025/Sep/18/agents/
3. Stack Overflow Developer Survey 2026, AI data. Stack Overflow. Oct 2026. https://survey.stackoverflow.co/2026/ai/data
4. 2026: The State of Consumer AI. Menlo Ventures (investor). 16 Sep 2026. https://menlovc.com/perspective/2026-the-state-of-consumer-ai/
5. AI coding agent adoption 2026. JetBrains Research (vendor). 18 Aug 2026. https://blog.jetbrains.com/research/2026/08/ai-coding-agent-adoption-2026/
6. MirrorCode. Epoch AI (with METR). 2026, exact date not stated. https://epoch.ai/mirrorcode
7. My AI Adoption Journey. mitchellh.com. 5 Feb 2026. https://mitchellh.com/writing/my-ai-adoption-journey
8. DeepTRACE audit (arXiv 2509.04499). arXiv. 2 Sep 2025. https://arxiv.org/abs/2509.04499
9. Significant increase in digital labor automation (Remote Labor Index). Center for AI Safety. 1 Jul 2026. https://safe.ai/blog/significant-increase-in-digital-labor-automation
10. Altman predicts AI agents will join workforce soon. eWeek. date not captured. https://www.eweek.com/news/altman-predicts-ai-agents-will-join-workforce-soon/
11. The Plunging Price of Thought. Epoch AI. 22 Sep 2026. https://epoch.ai/publications/the-plunging-price-of-thought
12. Time Horizons. METR. updated 8 Sep 2026. https://metr.org/time-horizons/
13. SpaceX just rolled Grok, Cursor and X into one subscription. 24/7 Wall St.. 13 Oct 2026. https://247wallst.com/investing/2026/10/13/spacex-just-rolled-grok-cursor-and-x-into-one-subscription-the-top-tier-is-200-a-month/
14. Building effective agents. Anthropic (vendor). 19 Dec 2024, modified 9 Oct 2026. https://www.anthropic.com/engineering/building-effective-agents
15. A practical guide to building agents. OpenAI (vendor). date not captured. https://cdn.openai.com/business-guides-and-resources/a-practical-guide-to-building-agents.pdf
16. Yang et al., agentic systems usage paper (arXiv 2512.07828). arXiv (Harvard and Perplexity authors). Dec 2025. https://arxiv.org/abs/2512.07828
17. DevDay 2026 Recap. OpenAI (vendor). date not captured; event 29 Sep 2026. https://openai.com/index/devday-2026-recap/
18. AI agents are moving into the small business mainstream. SBE Council. 30 Sep 2026. https://sbecouncil.org/2026/09/30/ai-agents-are-moving-into-the-small-business-mainstream/
19. AI Agent Standards Initiative. NIST. created 17 Feb 2026, updated 14 Aug 2026. https://www.nist.gov/artificial-intelligence/ai-agent-standards-initiative
20. Americans and AI 2026. Pew Research Center. 17 Jun 2026. https://www.pewresearch.org/internet/2026/06/17/americans-and-ai-2026-chatbots-smart-devices-and-views-on-impact/
21. How Much Code Do Developers Really Let Agents Write?. JetBrains Research (vendor). 26 Aug 2026. https://blog.jetbrains.com/research/2026/08/how-much-code-do-developers-really-let-agents-write/
22. Measuring AI agent autonomy in practice. Anthropic (vendor). 18 Feb 2026. https://www.anthropic.com/research/measuring-agent-autonomy
23. Future Workforce Index 2026. Upwork (vendor). 14 Jul 2026. https://www.upwork.com/research/research-future-workforce-index-2026
24. New Small Business Check-Up survey. SBE Council. 8 Oct 2026. https://sbecouncil.org/2026/10/08/new-small-business-check-up-survey-main-street-businesses-are-powering-through-2026/
25. AI Tooling for Software Engineers in 2026. The Pragmatic Engineer. 3 Mar 2026. https://newsletter.pragmaticengineer.com/p/ai-tooling-2026
26. Claude Code usage statistics 2026. Presenc AI (secondary). Oct 2026. https://presenc.ai/research/claude-code-usage-statistics-2026
27. Stewart et al., Figma Make trial (arXiv 2609.26725). arXiv (authors at Figma). 22 Sep 2026. https://arxiv.org/html/2609.26725
28. Ju and Aral, human-AI advertising trial (arXiv 2503.18238). arXiv; Organization Science 37(2). 2026. https://arxiv.org/html/2503.18238
29. AI agents complete 80% of shopping tasks across 50 Indian e-commerce sites. Social Samosa, reporting FTA Global. 6 Oct 2026. https://www.socialsamosa.com/industry-updates/ai-agents-complete-80-of-shopping-tasks-across-50-indian-e-commerce-sites-report-12629205
30. Agentic Engineering Patterns. simonwillison.net. begun 23 Feb 2026. https://simonwillison.net/guides/agentic-engineering-patterns/
31. Vibe Check: Claude Cowork is Claude Code for the rest of us. Every. 13 Jan 2026. https://every.to/vibe-check/vibe-check-claude-cowork-is-claude-code-for-the-rest-of-us
32. I let AI agents run my YouTube channel for 6 weeks. DEV Community. 16 Feb 2026. https://dev.to/wcamon/i-let-ai-agents-run-my-youtube-channel-for-6-weeks-heres-what-actually-happened-21b1
33. Early-2025 AI and experienced open-source developer study. METR. 10 Jul 2025. https://metr.org/blog/2025-07-10-early-2025-ai-experienced-os-dev-study/
34. Uplift update. METR. 24 Feb 2026. https://metr.org/blog/2026-02-24-uplift-update/
35. He et al., Cursor adoption study (arXiv 2511.04427). arXiv; MSR 2026. Apr 2026. https://arxiv.org/html/2511.04427
36. Agarwal, He and Vasilescu, agents versus IDE tools (arXiv 2601.13597). arXiv. Jan 2026. https://arxiv.org/abs/2601.13597
37. Many SWE-bench-passing PRs would not be merged into main. METR. 10 Mar 2026. https://metr.org/notes/2026-03-10-many-swe-bench-passing-prs-would-not-be-merged-into-main/
38. Karpathy on the decade before agents work. Fortune. 20 Oct 2025. https://dc.fortune.com/2025/10/20/workers-fear-ai-job-cuts-open-ai-co-founder-says-ai-agents-will-take-a-decade-before-they-even-work-they-dont-have-enough-intelligence-unemployment-automation-2035
39. GDPval leaderboard. AnotherWrapper (secondary). date not captured. https://anotherwrapper.com/tools/llm-pricing/evals/gdpval
40. What do economic value benchmarks tell us?. Epoch AI. 14 Feb 2026. https://epochai.substack.com/p/what-do-economic-value-benchmarks
41. AI Index 2026, Technical Performance. Stanford HAI. Apr 2026. https://hai.stanford.edu/ai-index/2026-ai-index-report/technical-performance
42. OSWorld 2.0 (arXiv 2606.29537). arXiv (Snorkel AI involved). 28 Jun 2026, revised 13 Jul 2026. https://arxiv.org/abs/2606.29537
43. MirrorCode preliminary results. Epoch AI. Apr 2026. https://epoch.ai/publications/mirrorcode-preliminary-results/
44. Amodei on AI writing code. Fortune. 13 Mar 2025. https://www.fortune.com/2025/03/13/ai-transforming-software-development-jobs-meta-ibm-anthropic
45. Anthropic CEO Dario Amodei on AI-generated code. ITPro. date not captured. https://itpro.com/technology/artificial-intelligence/anthropic-ceo-dario-amodei-ai-generated-code
46. AI usage survey. METR. 11 May 2026. https://metr.org/blog/2026-05-11-ai-usage-survey/
47. Audit of agent benchmark traces (arXiv 2607.22368). arXiv. 24 Jul 2026. https://arxiv.org/abs/2607.22368
48. Agent self-assessment study (arXiv 2602.06948). arXiv. 6 Feb 2026. https://arxiv.org/abs/2602.06948
49. Gartner predicts over 40% of agentic AI projects will be canceled by end of 2027. Gartner (enterprise). 25 Jun 2025. https://www.gartner.com/en/newsroom/press-releases/2025-06-25-gartner-predicts-over-40-percent-of-agentic-ai-projects-will-be-canceled-by-end-of-2027
50. The results of the 2026 Developer Survey are here. Stack Overflow blog. 6 Oct 2026. https://stackoverflow.blog/2026/10/06/the-results-of-the-2026-developer-survey-are-here/
51. OpenAI agentic shopping pullback. CNBC. 20 Mar 2026. https://www.cnbc.com/2026/03/20/open-ai-agentic-shopping-etsy-shopify-walmart-amazon.html
52. ChatGPT Atlas vs Perplexity Comet vs Gemini in Chrome. Tech Insider. 3 Sep 2026. https://tech-insider.org/ca/chatgpt-atlas-vs-perplexity-comet-vs-gemini-chrome-2026/
53. openclaw/openclaw repository. GitHub. read 30 Oct 2026. https://github.com/openclaw/openclaw
54. Exposed Moltbook database reveals millions of API keys. Wiz (security vendor). 2 Feb 2026. https://www.wiz.io/blog/exposed-moltbook-database-reveals-millions-of-api-keys
55. SlopCodeBench (arXiv 2603.24755), v2. arXiv. 7 May 2026. https://arxiv.org/abs/2603.24755
56. GPT-5.6 Sol evaluation. METR. 26 Jun 2026. https://metr.org/blog/2026-06-26-gpt-5-6-sol/
57. METR. Wikipedia (secondary). accessed 30 Oct 2026. https://en.wikipedia.org/wiki/METR
58. Time horizon limitations. METR. 22 Jan 2026. https://metr.org/notes/2026-01-22-time-horizon-limitations/
59. Anthropic ends subscription coverage for OpenClaw. The Next Web. 4 Apr 2026. https://thenextweb.com/news/anthropic-openclaw-claude-subscription-ban-cost
60. Usage-based billing for individuals. GitHub Docs (vendor). read 30 Oct 2026. https://docs.github.com/en/copilot/concepts/billing/usage-based-billing-for-individuals
61. Copilot credit complaints keep coming. Visual Studio Magazine. 7 Aug 2026. https://visualstudiomagazine.com/articles/2026/08/07/copilot-credit-complaints-keep-coming-too-expensive-to-use.aspx
62. Claude Code costs documentation. Anthropic (vendor). date not captured. https://code.claude.com/docs/en/costs
63. AI agents can now complete 16 percent of freelance jobs at pro quality. The Decoder. 2 Jul 2026. https://the-decoder.com/ai-agents-can-now-complete-16-percent-of-freelance-jobs-at-pro-quality-up-from-2-5-percent-eight-months-ago/
64. AI workslop: Zapier survey. IT Brief, reporting Zapier (vendor, enterprise). 2026. https://itbrief.com.au/story/ai-workslop-zapier-survey-finds-ai-delivers-gains-as-well-as-costly-corrections
65. Claude Code auto mode. Anthropic Engineering (vendor). 25 Mar 2026. https://www.anthropic.com/engineering/claude-code-auto-mode
66. AI cuts coding time but it's also filling open source's inbox. The Register, reporting Linux Foundation survey. 21 Oct 2026. https://www.theregister.com/ai-and-ml/2026/10/21/ai-cuts-coding-time-but-its-also-filling-open-sources-inbox-with-crap/5304389
67. The end of the curl bug bounty. daniel.haxx.se. 26 Jan 2026. https://daniel.haxx.se/blog/2026/01/26/the-end-of-the-curl-bug-bounty/
68. Prompt injection is not SQL injection. UK NCSC. 8 Dec 2025. https://www.ncsc.gov.uk/blog-post/prompt-injection-is-not-sql-injection
69. Careful Adoption of Agentic AI Services. ASD's ACSC and Five Eyes partners. May 2026. https://www.cyber.gov.au/business-government/secure-design/artificial-intelligence/careful-adoption-of-agentic-ai-services
70. Running OpenClaw safely. Microsoft Security (vendor). 19 Feb 2026. https://www.microsoft.com/en-us/security/blog/2026/02/19/running-openclaw-safely-identity-isolation-runtime-risk/
71. ToxicSkills: malicious AI agent skills on ClawHub. Snyk (security vendor). 5 Feb 2026. https://snyk.io/blog/toxicskills-malicious-ai-agent-skills-clawhub/
72. Researchers find 341 malicious ClawHub skills. The Hacker News, reporting Koi Security (vendor). 2 Feb 2026. https://thehackernews.com/2026/02/researchers-find-341-malicious-clawhub.html
73. Rogue AI agent Cursor goes haywire, deletes tech company's database. ABC30 Fresno. 30 Apr 2026. https://abc30.com/post/rogue-ai-agent-cursor-goes-haywire-deletes-tech-companys-database/19008099/
74. AI deletes entire company database and all backups in 9 seconds. PC Gamer. 28 Apr 2026. https://www.pcgamer.com/software/ai/here-we-go-again-ai-deletes-entire-company-database-and-all-backups-in-9-seconds-then-cheerfully-admits-i-violated-every-principle-i-was-given/
75. Claude Cowork exfiltrates files. PromptArmor (security vendor). about Jan 2026. https://www.promptarmor.com/resources/claude-cowork-exfiltrates-files
76. The 2025 AI Agent Index (PDF). MIT-hosted. 2026. https://aiagentindex.mit.edu/data/2025-AI-Agent-Index.pdf
77. Agentic AI Foundation surpasses 300 members. Agentic AI Foundation. 22 Oct 2026. https://aaif.io/news/agentic-ai-foundation-surpasses-300-members
78. Agentic AI Foundation announces four new projects. Linux Foundation. 22 Oct 2026. https://www.linuxfoundation.org/press/agentic-ai-foundation-announces-four-new-projects-agent-skills-open-responses-openenv-and-opensandbox
79. MCP Dev Summit 2026 readout. Digital Applied. Jun 2026. https://www.digitalapplied.com/blog/mcp-dev-summit-2026-readout-protocol-roadmap-analysis
80. Google Gemini Spark agentic assistant. The Next Web. date not captured. https://thenextweb.com/news/google-gemini-spark-agentic-assistant-gmail-io-2026
81. iOS 27 Siri AI has a waitlist. MacRumors. 15 Sep 2026. https://www.macrumors.com/2026/09/15/ios-27-siri-ai-has-waitlist-how-to-join/
82. Siri AI will launch in beta, complicated by daily usage caps. AppleInsider. 9 Sep 2026. https://appleinsider.com/articles/26/09/09/siri-ai-will-launch-in-beta-complicated-by-daily-usage-caps-future-paid-access
83. Meta debuts its Muse AI agent. TechCrunch. 8 Sep 2026. https://techcrunch.com/2026/09/08/meta-debuts-its-muse-ai-agent-will-consumers-trust-it/
84. Gemini Spark Chrome auto browse. 9to5Google. 30 Jul 2026. https://9to5google.com/2026/07/30/gemini-spark-chrome-auto-browse/
85. The AI Act implementation timeline under the AI Omnibus. Future of Privacy Forum. 28 Jul 2026, updated 5 Aug 2026. https://fpf.org/blog/the-ai-act-implementation-timeline-what-changes-under-the-ai-omnibus/
86. Ninth Circuit vacates CFAA injunction against Perplexity's Comet AI agent. Jones Day. Sep 2026. https://www.jonesday.com/en/insights/2026/09/ninth-circuit-vacates-cfaa-injunction-against-perplexitys-comet-ai-agent
87. AI cloud stocks fall as Big Tech capex comes in light. 24/7 Wall St.. 29 Oct 2026. https://247wallst.com/investing/2026/10/29/ai-cloud-stocks-fall-as-big-tech-capex-comes-in-light-fastly-sinks-6-oracle-and-nebius-drop-3/
88. Gartner predicts AI inference costs per agentic workflow will increase more than fivefold through 2028. Gartner (enterprise). 17 Aug 2026. https://www.gartner.com/en/newsroom/press-releases/2026-08-17-gartner-predicts-ai-inference-costs-per-agentic-workflow-will-increase-more-than-fivefold-through-2028
89. What the 2026 Hype Cycle for Agentic AI Reveals. Gartner (enterprise). 15 Apr 2026. https://www.gartner.com/en/articles/hype-cycle-for-agentic-ai
90. Timelines shrink in AI Futures quarterly. AI Stop Watch. 2026, exact date not captured. https://aistop.watch/p/timelines-shrink-in-ai-futures-quarterly
91. AI Futures Project. Wikipedia (secondary). date not captured. https://en.wikipedia.org/wiki/AI_Futures_Project
92. OpenAI's Codex and ChatGPT Work cross 10 million weekly users. Startup Fortune. date not captured. https://startupfortune.com/openais-codex-and-chatgpt-work-just-crossed-10-million-weekly-users-and-the-coding-wars-have-a-new-shape/
93. Every says Codex and ChatGPT for Work have 40 million weekly users combined. Superpower Daily. date not captured. https://superpowerdaily.com/posts/every-says-codex-and-chatgpt-for-work-have-40-million-weekly-users-combined
94. APEX-Agents (arXiv 2601.14242). arXiv (Mercor, vendor). Jan-Feb 2026. https://arxiv.org/abs/2601.14242
95. APEX-Agents 1.1 mirror. BenchLM (third-party mirror). snapshot 7 Oct 2026. https://benchlm.ai/benchmarks/mercorapexagents11
96. Time Horizon 1.1. METR. 29 Jan 2026. https://metr.org/blog/2026-01-29-time-horizon-1-1/
97. METR Time Horizon 2.0 (AI-written parody, not a METR release). EA Forum. 8 Jul 2026. https://forum.effectivealtruism.org/posts/ghhJh6SBYXxDktnZX/metr-time-horizon-2-0-the-benchmark-you-ve-been-waiting-for
98. How accurate is Perplexity Deep Research mode? (source of the unverified Haus claim). Perplexity AI Magazine. date not captured. https://perplexityaimagazine.com/perplexity-hub/how-accurate-is-perplexity-deep-research-mode/
99. Google I/O 2026 keynote. Google (vendor). May 2026. https://blog.google/innovation-and-ai/sundar-pichai-io-2026/

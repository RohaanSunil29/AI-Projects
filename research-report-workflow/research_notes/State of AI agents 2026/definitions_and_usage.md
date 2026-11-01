# What counts as an AI agent in 2026, and how individuals, creators and small teams actually use them

Notes as of 30 October 2026. Each citation gives publisher, title and date. "Vendor-published" means the publisher sells or invests in the product category it is measuring. "Secondary" means I read the number in an aggregator or press piece, not the primary source. Percentages calculated by me are in Inferences and are marked as calculations.

## How do credible sources define an AI agent in 2026, and what separates an agent from a chatbot, a copilot or a scripted automation?

### Takeaway
Sources converge on one working core: an LLM that controls its own sequence of actions, using tools, in pursuit of a goal, and that can change something outside the conversation. They disagree on how much autonomy qualifies, on whether predefined workflows count, and on whether an agent must keep working unattended. No binding standards-body definition turned up: NIST has an agent programme but its pages describe agents only in passing.

### Cited Findings

**Standards and public bodies**
- NIST describes agents only as "the next generation of AI—agents capable of autonomous actions" that "function securely on behalf of users and interoperate smoothly across the digital landscape"; the initiative page sets out pillars (industry standards, open protocols, security and identity research) and no formal definition — [NIST, AI Agent Standards Initiative, created 17 Feb 2026, updated 14 Aug 2026](https://www.nist.gov/artificial-intelligence/ai-agent-standards-initiative)
- A US financial-sector lexicon defines an AI agent as "A system that autonomously perceives its environment, decides what to do, and takes actions to achieve its goals," and agentic AI as a category "capable of independently making decisions, interacting with their environment, and optimizing processes without direct human intervention." Read from a search excerpt only — [Artificial Intelligence Executive Oversight Group, AI Lexicon, Feb 2026, hosted by FSSCC](https://fsscc.org/wp-content/uploads/2026/02/AIEOG-AI-Lexicon-February-2026.pdf)

**Independent researchers**
- The AI Agent Index has the most operational test found. It requires all four of: (1) autonomy of at least "L2", where "user and agent collaboratively plan, delegate, and execute"; (2) goal complexity, in practice "at least three autonomous tool calls and high-level task specification without step-by-step instructions"; (3) environmental interaction, in practice "write access to a computer and the ability to choose tools"; (4) generality across related tasks rather than one narrow function. It also applies impact criteria, such as at least 20,000 GitHub stars for open-source projects — [The 2025 AI Agent Index, arXiv 2602.17753, Feb 2026 by arXiv ID](https://arxiv.org/html/2602.17753v1)
- The Index covers 30 agents and found that most safety-related fields (135 of 240) had no public information — [The 2025 AI Agent Index PDF, MIT-hosted, 2026](https://aiagentindex.mit.edu/data/2025-AI-Agent-Index.pdf)
- Practitioner definition: "An LLM agent runs tools in a loop to achieve a goal." Willison argues this is now usable jargon among technical implementers but says other audiences need the definition clarified — [Simon Willison's Weblog, 18 Sep 2025](https://simonwillison.net/2025/Sep/18/agents/)

**Leading labs (vendor-published)**
- Anthropic: workflows are "systems where LLMs and tools are orchestrated through predefined code paths"; agents are "systems where LLMs dynamically direct their own processes and tool usage, maintaining control over how they accomplish tasks." It calls both "agentic systems", and describes agents as "typically just LLMs using tools based on environmental feedback in a loop" — [Anthropic, Building effective agents, 19 Dec 2024, page modified 9 Oct 2026, with a note that tooling has changed since 2024](https://www.anthropic.com/engineering/building-effective-agents)
- OpenAI: "Agents are systems that independently accomplish tasks on your behalf." It excludes applications that "integrate LLMs but don't use them to control workflow execution—think simple chatbots, single-turn LLMs, or sentiment classifiers" — [OpenAI, A practical guide to building agents, publication date not shown in my extract](https://cdn.openai.com/business-guides-and-resources/a-practical-guide-to-building-agents.pdf)
- OpenAI's 2026 consumer framing adds persistence: Dots are "always-on agents" that are "always working on your behalf" — [OpenAI, DevDay 2026 Recap, page date not shown in my extract; DevDay was 29 Sep 2026 per fatjoe](https://openai.com/index/devday-2026-recap/). Meta's Muse is similarly described as an agent "that can continue working on tasks after a conversation ends" — [SBE Council, 30 Sep 2026](https://sbecouncil.org/2026/09/30/ai-agents-are-moving-into-the-small-business-mainstream/)
- Perplexity and Harvard Business School: agentic systems are "AI assistants capable of autonomously pursuing user-defined goals by planning and taking multi-step actions on a user's behalf to interact with and effect outcomes across real-world environments". The paper stresses the ability to "actively modify" the environment, and says agents "extend chatbots' capabilities beyond conversations to include autonomous actions" — [Yang et al., arXiv 2512.07828, v2 10 Dec 2025, Harvard and Perplexity authors](https://arxiv.org/html/2512.07828v2)

**Analysts and investors**
- Gartner's three-way rule of thumb: "using AI agents when decisions are needed, automation for routine workflows and assistants for simple retrieval." It says many use cases sold as agentic "don't require agentic implementations" — [Gartner press release, 25 Jun 2025](https://www.gartner.com/en/newsroom/press-releases/2025-06-25-gartner-predicts-over-40-percent-of-agentic-ai-projects-will-be-canceled-by-end-of-2027)
- Menlo Ventures: "AI agents can reason, make decisions, complete multi-step tasks, and take actions in other systems" — [Menlo Ventures, 2026: The State of Consumer AI, 16 Sep 2026, vendor-published](https://menlovc.com/perspective/2026-the-state-of-consumer-ai/)

**Where sources disagree**
- On workflows: Anthropic's umbrella "agentic systems" includes predefined workflows, while OpenAI requires the LLM to control execution and Gartner reserves agents for decision work ([Anthropic](https://www.anthropic.com/engineering/building-effective-agents); [OpenAI](https://cdn.openai.com/business-guides-and-resources/a-practical-guide-to-building-agents.pdf); [Gartner](https://www.gartner.com/en/newsroom/press-releases/2025-06-25-gartner-predicts-over-40-percent-of-agentic-ai-projects-will-be-canceled-by-end-of-2027))
- On autonomy: the Agent Index accepts collaborative L2 systems, while the AIEOG lexicon says "without direct human intervention" ([AI Agent Index](https://arxiv.org/html/2602.17753v1); [AIEOG](https://fsscc.org/wp-content/uploads/2026/02/AIEOG-AI-Lexicon-February-2026.pdf))
- On terminology: Perplexity's paper notes that its team prefers "assistant" over "agent", the word many sources use for the less capable category ([Yang et al.](https://arxiv.org/html/2512.07828v2); [Gartner](https://www.gartner.com/en/newsroom/press-releases/2025-06-25-gartner-predicts-over-40-percent-of-agentic-ai-projects-will-be-canceled-by-end-of-2027))

### Inferences
- A workable test across these sources has four parts: (1) the user states a goal rather than steps; (2) the model chooses the next action; (3) it can use tools with write access, so it changes something outside the chat; (4) it loops on results until a stopping condition. Persistence (runs unattended, keeps going after the chat ends) is emerging as a fifth, optional trait, and is not yet part of any formal definition I found.
- The distinctions that follow from that test are mine, synthesised from the sources above:

| Type | Who decides the next step | Acts outside the conversation? | Example in this research |
|---|---|---|---|
| Chatbot | Human, turn by turn | No, or read-only | Single-turn answers |
| Copilot / assistant | Human; AI suggests inside a tool | Limited; the human accepts each change | Inline code completion |
| Scripted automation / workflow | The developer, in advance | Yes, on fixed paths | A rule-based automation; RPA |
| Agent | The model, within limits | Yes, with tool choice | Coding agents, browser agents |

- Products cross these lines by mode. A single product can be a chatbot in one mode and an agent in another, so counts by product name overstate agent use.

### Gaps
- I did not verify the ISO/IEC wording. One secondary page says ISO defines the term and the EU AI Act does not use it ([The SuperSkills, undated excerpt](https://thesuperskills.com/research/what-is-an-ai-agent)); treat as unconfirmed.
- I could not retrieve Gartner's formal definition: its "AI agents" URL redirects to a CIO article and the query returned no definition text.
- No OECD definition was found in the single search I ran.
- A formal NIST definition may exist in its RFI or concept paper, which I did not read.

## What is "agent washing", and what evidence exists on how common it is?

### Takeaway
"Agent washing" is Gartner's term for relabelling existing assistants, RPA and chatbots as agents. The only widely cited prevalence figure is one Gartner estimate from June 2025, with no published method, about the enterprise vendor market: about 130 real vendors out of "thousands". I found no measured prevalence for consumer or small-team products, and no updated figure.

### Cited Findings
- Gartner defines it as "the rebranding of existing products, such as AI assistants, robotic process automation (RPA) and chatbots, without substantial agentic capabilities" and states: "Gartner estimates only about 130 of the thousands of agentic AI vendors are real." The press release gives no method or count of the denominator — [Gartner press release, 25 Jun 2025](https://www.gartner.com/en/newsroom/press-releases/2025-06-25-gartner-predicts-over-40-percent-of-agentic-ai-projects-will-be-canceled-by-end-of-2027)
- Gartner also predicted over 40% of agentic AI projects will be cancelled by end of 2027 (a forecast, not a measurement) — [same release, 25 Jun 2025](https://www.gartner.com/en/newsroom/press-releases/2025-06-25-gartner-predicts-over-40-percent-of-agentic-ai-projects-will-be-canceled-by-end-of-2027)
- In April 2026 Gartner placed agentic AI at the Peak of Inflated Expectations: only 17% of organisations had deployed AI agents and more than 60% expected to within two years. Most deployments "remain narrowly scoped" and fully autonomous agents "are not ready for the majority of enterprise use cases." The public article does not repeat the 130 figure — [Gartner, What the 2026 Hype Cycle for Agentic AI Reveals, 15 Apr 2026](https://www.gartner.com/en/articles/hype-cycle-for-agentic-ai)
- A vendor blog says Gartner's Hype Cycle calls out agent washing as a market problem; the full report is gated and this is unverified — [xpander.ai, 2026, secondary](https://xpander.ai/blog/gartner-hype-cycle-for-agentic-ai-what-it-means-for-ai-agent-development-platforms)

**Loose labelling in the data itself (evidence of label drift, not of deceptive marketing)**
- Stack Overflow's "Where technologists look for answers" chart reports 70% "Ask an AI agent" as a way of seeking answers, which in my reading is mostly chat-style lookup — [Stack Overflow blog, 6 Oct 2026](https://stackoverflow.blog/2026/10/06/the-results-of-the-2026-developer-survey-are-here/)
- The same survey has a single category, "AI agents or automated workflows" (26.2%), and its automation question is led by Make (38.9%), n8n (32.7%) and Zapier (18.5%) among 4,173 respondents — [Stack Overflow Developer Survey 2026, AI data, Oct 2026](https://survey.stackoverflow.co/2026/ai/data)
- JetBrains' "AI coding agents" count and its product list include GitHub Copilot and Cursor, with no breakdown of agent mode against autocomplete in the post — [JetBrains Research, 18 Aug 2026](https://blog.jetbrains.com/research/2026/08/ai-coding-agent-adoption-2026/)
- Menlo says 32% of AI users have let AI act without final sign-off and that "many don't think of this as 'using an agent'", which shows under-labelling as well as over-labelling — [Menlo Ventures, 16 Sep 2026, vendor-published](https://menlovc.com/perspective/2026-the-state-of-consumer-ai/)

**Disagreement on how much agent activity is real**
- Small employers: 58% report using AI agents regularly or occasionally ([SBE Council, 8 Oct 2026, n=516, firms with 2 to 99 employees](https://sbecouncil.org/2026/10/08/new-small-business-check-up-survey-main-street-businesses-are-powering-through-2026/)). Organisations overall: 17% have deployed agents ([Gartner, 15 Apr 2026](https://www.gartner.com/en/articles/hype-cycle-for-agentic-ai)). Enterprise functions: scaled use "in the single digits" in almost all functions, from a 2025 McKinsey survey ([Stanford HAI, AI Index 2026, Chapter 4, 2026](https://hai.stanford.edu/assets/files/ai_index_report_2026_chapter_4_economy.pdf))

### Inferences
- The "130 of thousands" figure should be quoted as an analyst's rough estimate from 16 months ago, not as a finding. It implies under about 13% if "thousands" means at least 1,000, and that bound is my arithmetic, not Gartner's.
- For individuals the bigger problem may be label confusion rather than fraud. Surveys ask people about "agents" in a market where the word covers chat lookup, automation tools and coding agents.
- The 58% against 17% gap is unlikely to mean small firms are far ahead of enterprises. "Occasionally using" an agent and "deploying" one are different bars, and small-business respondents may count ordinary AI features.

### Gaps
- No independent audit of consumer "agent" products against a functional test was found. This would be the direct measure of washing at the individual level.
- No regulator action specific to agent claims was searched for in depth.
- No update to Gartner's 130 figure was found.

## What are individuals, creators, freelancers and small teams actually using agents for?

### Takeaway
Coding is the best-evidenced and deepest use. Outside coding, the only telemetry-based study shows browser-agent use centred on productivity, learning and research, and shopping, with personal use the majority. Evidence specific to creators and freelancers is thin: most "creator" data measures AI use in general, not agents.

### Cited Findings

**Coding (best evidence)**
- Self-reported averages among professional developers: about 47% of code fully written by agents, 38% AI-assisted, 27% manual (buckets overlap, so the sum exceeds 100%). About 22% get over 80% of their code from agents; 31% are classed as "agentic coders", 47% "AI-assisted", 23% "manual" — [JetBrains Research, How Much Code Do Developers Really Let Agents Write?, 26 Aug 2026, survey May to Jul 2026, 15,000+ developers, vendor-published](https://blog.jetbrains.com/research/2026/08/how-much-code-do-developers-really-let-agents-write/)
- Tasks for "AI or AI agents" (not agents alone), n=12,547: generating code in a familiar area 69.3%, debugging 63.8%, simple questions 59.4%, tests 58.1%, unfamiliar code 56.0%, documentation 51.1%, internal knowledge search 49.7%, code review 40.5%, emails and messages 23.5%, deploying and operating production 19.9%, media assets 17.5% — [Stack Overflow Developer Survey 2026, AI data, Oct 2026](https://survey.stackoverflow.co/2026/ai/data)
- Output checking: 9.6% use AI output as-is; 76.5% run it locally. 48.0% trust AI only when they can easily verify it; 6.6% trust it for many tasks including important work decisions — [Stack Overflow Developer Survey 2026, AI data, Oct 2026](https://survey.stackoverflow.co/2026/ai/data)
- Autonomy telemetry: the 99.9th-percentile Claude Code turn rose from under 25 to over 45 minutes between Oct 2025 and Jan 2026, while "nearly every percentile below the 99th" stayed stable. Full auto-approve rises from about 20% of sessions for new users to over 40% for experienced users — [Anthropic, Measuring AI agent autonomy in practice, 18 Feb 2026, vendor-published](https://www.anthropic.com/research/measuring-agent-autonomy)
- On Anthropic's public API, about 73% of tool calls appeared to have a human in the loop, 0.8% appeared irreversible, and software engineering was about half of tool calls — [Latent Space, summarising Anthropic, Feb 2026, secondary](https://latent.space/p/ainews-anthropics-agent-autonomy/)

**General-purpose and browser agents**
- Comet Assistant, hundreds of millions of interactions: Productivity & Workflow plus Learning & Research are 57% of agentic queries; Courses plus Shopping for Goods are 22%; the top 10 of 90 tasks are 55%; personal use 55%, professional 30%, educational 16% — [Yang et al., arXiv 2512.07828, Dec 2025, co-authored by Perplexity staff](https://arxiv.org/abs/2512.07828)
- Six occupations make up 70% of agent activity. Digital technologists are 30% of queries; finance users put 47% of queries into productivity; students put 43% into learning and research — [Perplexity blog, How People Use AI Agents, Dec 2025, vendor-published](https://www.perplexity.ai/hub/blog/how-people-use-ai-agents)
- Framing disagreement: Perplexity's blog calls the 57% "cognitive work" ("a thinking partner more than a butler"), while the paper reports it only as the sum of two topic categories, which include generic productivity — [blog](https://www.perplexity.ai/hub/blog/how-people-use-ai-agents); [paper](https://arxiv.org/abs/2512.07828)
- US consumers granting access to agents: email 36%, browsers 33%, messaging 31%, cloud storage 29%, calendars 27%, health apps 23%, financial accounts 20% — [Menlo Ventures, 16 Sep 2026, n=5,067, Morning Consult, Jul 2026, vendor-published](https://menlovc.com/perspective/2026-the-state-of-consumer-ai/)
- Among AI-using shoppers: 50% compare prices, 43% narrow a shortlist, 37% made a final decision on AI's recommendation, 26% let AI complete a purchase — [Menlo Ventures, 16 Sep 2026, vendor-published](https://menlovc.com/perspective/2026-the-state-of-consumer-ai/)

**Freelancers and creators**
- 41% of freelancers report "using AI agents for autonomous task execution" against 34% of full-time employees — [Upwork, Future Workforce Index 2026, 14 Jul 2026, 2,400 US workers, Mar to Apr 2026, vendor-published: Upwork runs a freelance marketplace](https://www.upwork.com/research/research-future-workforce-index-2026)
- 48% of AI users say they have earned money with AI, most commonly content creation (22%) and freelancing (18%); 62% of Gen Z AI users against 15% of Boomer AI users. This is AI use in general, not agents — [Menlo Ventures, 16 Sep 2026, vendor-published](https://menlovc.com/perspective/2026-the-state-of-consumer-ai/)
- Share of people doing a creative activity who use AI for it: writing 61%, images 53%, presentations 52%, game creation 52%, video 44%. Again general AI — [Menlo Ventures, 16 Sep 2026, vendor-published](https://menlovc.com/perspective/2026-the-state-of-consumer-ai/)

**Small teams and solo operators**
- Among the smallest companies in a newsletter survey: Claude Code 75%, chatbots 55%, Cursor 42%, GitHub Copilot 35%, Codex 26%, Gemini CLI 14%, OpenCode 13%. Overall, 55% of respondents regularly use agents (507 of 906). Presenc reports the band as 1 to 50 people — [The Pragmatic Engineer, AI Tooling for Software Engineers in 2026, 3 Mar 2026, fielded 27 Jan to 17 Feb 2026, paywalled, public portion only](https://newsletter.pragmaticengineer.com/p/ai-tooling-2026); [Presenc AI, Oct 2026, secondary](https://presenc.ai/research/claude-code-usage-statistics-2026)
- Stack Overflow says it has "heard anecdotally" of people using agents to "soloprenuer their way to a viable company", and offers its data as possible support; this is a suggestion, not a measurement — [Stack Overflow blog, 6 Oct 2026](https://stackoverflow.blog/2026/10/06/the-results-of-the-2026-developer-survey-are-here/)
- Small-business use cases listed by SBE Council (illustrative, not measured): analysing sales and marketing results, preparing campaigns, flagging customer issues, organising scattered data, reviewing finances, tracking emails and calendars — [SBE Council, 30 Sep 2026](https://sbecouncil.org/2026/09/30/ai-agents-are-moving-into-the-small-business-mainstream/)
- Low-code app builders among developers who answered (n=2,219): Lovable 38.3%, Replit 28.3%, v0 27.5%, Bolt.new 17.2% — [Stack Overflow Developer Survey 2026, AI data, Oct 2026](https://survey.stackoverflow.co/2026/ai/data)

### Inferences
- Use is split: a deep, long-running tail of technical users and a broad base with short, supervised tasks. Anthropic's percentiles and JetBrains' 22% both point this way.
- Delegation is mainly of reversible work that can be checked. Stack Overflow's 19.9% for production operations and 48% "when I can verify it" fit this, as does the 0.8% irreversible figure.
- Comet data predate most 2026 agent launches and come from one browser's early adopters, so they should not be generalised to all consumers.
- Scheduling and personal-assistant agents are evident from access-permission data, but I found no direct measure of how often those tasks are done.

### Gaps
- No independent dataset on creators' use of agents specifically (as opposed to generative tools) was found.
- No representative survey of small teams (2 to 10 people) outside software was found. SBE Council covers firms with 2 to 99 employees, and its 58% is a single top-line figure from an advocacy group.
- Newer lab usage studies from 2026 were not searched exhaustively. OpenAI's "How People Use ChatGPT" (NBER 34255, Sep 2025) concerns chat, not agents, and I saw it only as cited by Menlo.

## What do adoption numbers show, separating people who tried an agent from people who use one regularly?

### Takeaway
Among all US adults, regular agent use is a minority behaviour. The best consumer estimate is 41% of AI users tried and 24% regular, from an investor's survey, which I calculate as roughly 26% and 15% of US adults. Developers are the exception, where agents are daily practice for many, but the figures range widely with the definition: about 17% to 68% daily.

### Cited Findings

| Population | Source and date | Aware | Tried or any use | Regular | Daily |
|---|---|---|---|---|---|
| US AI users | Menlo, Jul 2026 survey | 72% | 41% | 24% | Not given for agent use |
| Professional developers worldwide | JetBrains, May to Jul 2026 | n/a | n/a | 90% weekly or more | 68% |
| Stack Overflow respondents | SO, Jun to Aug 2026 | n/a | 26.2% "AI agents or automated workflows" | see Inferences | 63.1% of those users |
| Stack Overflow respondents, coding assistants or agents | SO, Jun to Aug 2026 | n/a | 65.9% | n/a | 73.0% of those users |
| Newsletter developer readers | Pragmatic Engineer, Jan to Feb 2026 | n/a | n/a | 55% | n/a |
| US workers | Upwork, Mar to Apr 2026 | n/a | 41% freelancers, 34% full-time | n/a | n/a |
| US small employers | SBE Council, Sep 2026 | n/a | 58% regularly or occasionally; another 14% considering | n/a | n/a |

Sources for the table: [Menlo Ventures, 16 Sep 2026, vendor-published](https://menlovc.com/perspective/2026-the-state-of-consumer-ai/); [JetBrains, 18 Aug 2026, vendor-published](https://blog.jetbrains.com/research/2026/08/ai-coding-agent-adoption-2026/); [Stack Overflow, AI data, Oct 2026](https://survey.stackoverflow.co/2026/ai/data); [The Pragmatic Engineer, 3 Mar 2026](https://newsletter.pragmaticengineer.com/p/ai-tooling-2026); [Upwork, 14 Jul 2026, vendor-published](https://www.upwork.com/research/research-future-workforce-index-2026); [SBE Council, 8 Oct 2026](https://sbecouncil.org/2026/10/08/new-small-business-check-up-survey-main-street-businesses-are-powering-through-2026/).

**Consumer detail**
- Menlo: survey of 5,067 US adults with Morning Consult, July 2026, weighted to be nationally representative. AI use moved from 61.0% to 63.6% between 2025 and 2026 and 55% of AI users pay. Agent questions are new, with no 2025 baseline. Awareness includes those who said they were unsure. Daily AI use is 39% of AI users overall against 63% of agent users; 65% of payers use an agent against 13% of non-payers — [Menlo Ventures, 16 Sep 2026, vendor-published](https://menlovc.com/perspective/2026-the-state-of-consumer-ai/)
- Menlo's bias: it is an investor, and marks portfolio companies with an asterisk, including Claude Code/Cowork and Hermes in its agent ranking — [Menlo Ventures, 16 Sep 2026](https://menlovc.com/perspective/2026-the-state-of-consumer-ai/)
- Pew's nearest measure is chatbots, not agents: 49% of US adults use AI chatbots, 24% daily (12% several times a day, 4% almost constantly), up from 33% ever-use in 2024 with changed question wording. The report's main page has no agent question; n=5,119, 17 to 23 Feb 2026 — [Pew Research Center, Americans and AI 2026, 17 Jun 2026](https://www.pewresearch.org/internet/2026/06/17/americans-and-ai-2026-chatbots-smart-devices-and-views-on-impact/)
- Gallup: 50% of US employees use AI at work at least a few times a year, 28% a few times a week or more, 13% daily. The article does not mention agents; n=23,717, 4 to 19 Feb 2026 — [Gallup, Rising AI Adoption Spurs Workforce Changes, 12 Apr 2026](https://www.gallup.com/workplace/704225/rising-ai-adoption-spurs-workforce-changes.aspx)

**Developer detail**
- Stack Overflow fielded 23 Jun to 5 Aug 2026 with 30,903 valid responses, recruited through its own site, blog and email list, so it is self-selected. The AI questions had smaller bases (for example n=17,464) — [Stack Overflow, Methodology 2026](https://survey.stackoverflow.co/2026/methodology); [AI data](https://survey.stackoverflow.co/2026/ai/data)
- Baseline, older data: in 2025, 52% of developers either did not use agents or stuck to simpler AI tools, and 38% had no plans to adopt them — [Stack Overflow Developer Survey 2025](https://survey.stackoverflow.co/2025/ai)
- Stack Overflow 2026: 17.2% do not use AI tools; 31% of daily AI users spend four or more hours a day with it (n=10,926) — [Stack Overflow, AI data, Oct 2026](https://survey.stackoverflow.co/2026/ai/data)
- JetBrains is reweighted by region, employment status, language and JetBrains familiarity, which should reduce but not remove its audience bias. Its survey covers more than 15,000 professional developers — [JetBrains, 18 Aug 2026](https://blog.jetbrains.com/research/2026/08/ai-coding-agent-adoption-2026/)

**Where sources disagree**
- Size of the AI-using population: Menlo 63.6% of US adults use AI; Pew 49% use chatbots. The questions differ (any AI product against chatbots). They agree closely on daily use: Menlo 25%, Pew 24% — [Menlo](https://menlovc.com/perspective/2026-the-state-of-consumer-ai/); [Pew](https://www.pewresearch.org/internet/2026/06/17/americans-and-ai-2026-chatbots-smart-devices-and-views-on-impact/)
- Growth: Menlo says adoption "hardly grew" in 2026 while Pew shows a large rise from 2024 to early 2026. Different windows and a wording change in Pew — same sources
- Developer agent use: JetBrains 90% weekly and 68% daily; Stack Overflow 26.2% for "AI agents or automated workflows" but 65.9% for "coding assistants or coding agents", and those are not separated — [JetBrains](https://blog.jetbrains.com/research/2026/08/ai-coding-agent-adoption-2026/); [Stack Overflow](https://survey.stackoverflow.co/2026/ai/data)
- A paywalled article reports that JetBrains' January wave also found 90% regularly using "at least one AI tool for coding" at work. If so, the same 90% now described as "agents" may reflect a broad definition — [Noor Mohammad, AI in Plain English, 23 Sep 2026, secondary](https://ai.plainenglish.io/three-surveys-three-1-coding-agents-claude-code-is-18-in-one-and-41-in-another-5b96b8925af4)

### Inferences
- Calculations from Menlo: 63.6% × 41% ≈ 26% of US adults have tried an agent, and 63.6% × 24% ≈ 15% use one regularly. Using Menlo's own scaling (55% of AI users ≈ 90M, so about 164M AI users), that is about 67M tried and 39M regular.
- Calculation: 24 ÷ 41 ≈ 59% of those who tried an agent report regular use. Self-reported and not a retention measure.
- Treat the 39M with caution. Menlo also says Codex is used by 35% of agent users. Applied to 39M that is about 14M US users, set against one secondary report of 20M weekly users worldwide for all of OpenAI's coding and work products. Possible, but it suggests over-reporting, likely from loose use of "agent". Menlo's sign-off finding pulls the other way (some real agentic use is not recognised as such). The error direction is therefore not certain.
- Menlo's numbers do not fully reconcile. 55% × 65% + 45% × 13% ≈ 41.6%, matching "tried", so its payer split seems to use the tried base. That implies about 86% of triers pay, not the stated 92% of "agent users", which may refer to a narrower group.
- Calculation from Stack Overflow: 26.2% × 63.1% ≈ 16.5% of respondents use "AI agents or automated workflows" daily. Bases differ somewhat, so this is approximate.
- Best framing: regular agent use is a paying-power-user behaviour in the general public, and normal practice among developers.

### Gaps
- No independent, probability-based survey with a defined "agent" question of the general public was found. Pew and Gallup materials I read do not ask it directly.
- I could not confirm whether Menlo showed respondents its definition of "agent"; the question wording was not in what I read.
- No published retention or churn data for any agent product was found.
- Reuters Institute and a16z consumer reports were not retrieved in this run. No non-US consumer agent adoption figure was found.
- The Stanford AI Index agent data I read are enterprise figures from McKinsey (2025), and are not individual-level.

## Which agent products have the most real-world usage among individuals as of late 2026?

### Takeaway
Claude Code leads developer surveys, and Codex is the fastest riser and leads Menlo's consumer agent question. No vendor reports audited, comparable agent-only user counts, so no definitive ranking exists. Browser and research agents have the weakest data. ChatGPT has by far the largest assistant audience, but that figure is not agent use.

### Cited Findings

**Coding agents**

| Tool | JetBrains: used at work, Jan 2026 | JetBrains: May to Jul 2026 | Stack Overflow 2026 "used" (n=12,255) |
|---|---|---|---|
| Claude Code | 18% | 39% (47% US; 31% main tool) | 65.5% |
| GitHub Copilot | 29% ("a year ago" per JetBrains) | 21% | 58.7% |
| OpenAI Codex | 3% | 16% | 29.5% |
| Cursor | 18% | 12% | 25.5% |
| OpenCode | n/a | 7% | 13.6% |
| Google Antigravity | n/a in this post | 6% | 16.0% |

Sources: [JetBrains, 18 Aug 2026, vendor-published](https://blog.jetbrains.com/research/2026/08/ai-coding-agent-adoption-2026/); [Stack Overflow, AI data, Oct 2026](https://survey.stackoverflow.co/2026/ai/data). The January column for Cursor comes from JetBrains and is restated by [Presenc AI, Oct 2026, secondary](https://presenc.ai/research/claude-code-usage-statistics-2026), which also lists Copilot at 29% for January.

- JetBrains' awareness figures: Codex rose from 27% to 65%; Copilot 79%; Cursor 75%; OpenCode 42%; Antigravity 47% — [JetBrains, 18 Aug 2026](https://blog.jetbrains.com/research/2026/08/ai-coding-agent-adoption-2026/)
- Developers who get over 80% of their code from agents: 42% of Codex users, 32% of those whose main tool is Claude Code, 28% of Cursor users — [JetBrains, 26 Aug 2026](https://blog.jetbrains.com/research/2026/08/how-much-code-do-developers-really-let-agents-write/)
- Claude Code absolute users: Anthropic has published none as of 1 Oct 2026, only that weekly actives doubled between 1 Jan and 12 Feb 2026. npm logged 55.8M downloads in the 30 days to 29 Sep 2026, a measure that includes updates and automated installs and so overstates people — [Presenc AI, Oct 2026, secondary, citing Anthropic and npm](https://presenc.ai/research/claude-code-usage-statistics-2026)
- Codex: 20M weekly users across OpenAI's coding and work products, per slides at an Aug 19 all-hands. Not confirmed by a primary source I read — [fatjoe, Oct 2026, secondary, low confidence](https://fatjoe.com/blog/chatgpt-stats/)
- Cursor: over 1M daily active users, attributed to CNBC, May 2026 — [Tech Insider, 2026, secondary](https://tech-insider.org/codex-vs-cursor-vs-claude-code-2026/). Copilot: 50M users on 4.7M paid seats, an aggregator figure — [IdeaPlan, verified Sep 2026, secondary](https://www.ideaplan.io/blog/ai-coding-assistant-market-share-2026)
- Sources describe the Pragmatic Engineer's 46/19/9 result differently: Presenc calls it "most loved" and IdeaPlan says it is share of mentions in an open-ended question, and that it corrected its own misattribution — [Presenc](https://presenc.ai/research/claude-code-usage-statistics-2026); [IdeaPlan](https://www.ideaplan.io/blog/ai-coding-assistant-market-share-2026)

**Consumer agent ranking (one survey)**
- Among agent users: Codex 35%, Claude Code/Cowork 32%, Perplexity 24%; Manus, OpenClaw and Hermes each 10 to 16%. Claude users are the most likely to run agents (48%, 1.5x ChatGPT or Gemini users) — [Menlo Ventures, 16 Sep 2026, vendor-published, investor in Anthropic and Hermes's maker per its portfolio markers](https://menlovc.com/perspective/2026-the-state-of-consumer-ai/)

**General assistants (reach, not agent use)**
- ChatGPT 1.2B weekly users — [OpenAI, DevDay 2026 Recap, vendor claim](https://openai.com/index/devday-2026-recap/)
- Share of US adults who ever use each: ChatGPT 44%, Gemini 24%, Copilot 17%, Meta AI 14%, Grok 8%, Claude 6% — [Pew, 17 Jun 2026, fielded Feb 2026](https://www.pewresearch.org/internet/2026/06/17/americans-and-ai-2026-chatbots-smart-devices-and-views-on-impact/)

**Browser agents**
- ChatGPT Atlas launched 21 Oct 2025; OpenAI announced deprecation on 9 Jul 2026, and it was scheduled to stop working on 9 Aug 2026, with features moved to the ChatGPT desktop app and browser extension — [Tech Insider, 3 Sep 2026, citing OpenAI Help Center](https://tech-insider.org/ca/chatgpt-atlas-vs-perplexity-comet-vs-gemini-chrome-2026/); [AI Toolbox, Sep 2026, citing OpenAI docs](https://www.ai-toolbox.co/chatgpt-management-and-productivity/chatgpt-atlas-browser-guide-2026)
- Claude for Chrome installs: about 40,000 in Dec 2025, 1M in Feb 2026, over 10M by Jun 2026. Installs are not active use — [searchVIU, 5 Aug 2026, citing Chrome Web Store](https://www.searchviu.com/en/ai-browsers-2026-compared/)
- Comet: about 18M monthly users by end of Q1 2026, from "third-party estimates" — [fatjoe, Oct 2026, secondary, low confidence](https://fatjoe.com/blog/perplexity-ai-stats/). Perplexity's over 100M monthly actives across all products comes from its CEO via Sacra — [Omnibound, 2026, secondary](https://www.omnibound.ai/blog/perplexity-ai-statistics)

**Open-source personal agents**
- GitHub stars on 30 Oct 2026: OpenClaw 393,425 (82,695 forks; repo created 24 Nov 2025); Hermes Agent 258,690 (56,832 forks; repo created 22 Jul 2025) — [GitHub, openclaw/openclaw](https://github.com/openclaw/openclaw); [GitHub, NousResearch/hermes-agent](https://github.com/NousResearch/hermes-agent)
- OpenClaw's stars went from about 247,000 on 2 Mar 2026 to 393,425 now, while one blog reports Google Trends interest collapsing in April after Anthropic ended Claude subscription access for third-party tools on 4 Apr 2026, and an estimated 135,000 instances running at peak — [Rost Glukhov, 27 Apr 2026, updated 5 Aug 2026, single-author blog](https://www.glukhov.org/ai-systems/openclaw/openclaw-rise-and-fall-timeline/)
- Star-speed claims conflict: "100,000 stars in under 48 hours" ([Glukhov](https://www.glukhov.org/ai-systems/openclaw/openclaw-rise-and-fall-timeline/)) against about two months ([LinkedIn post, 2026](https://www.linkedin.com/posts/uhb-ubs_openclaw-a-platform-that-enables-users-to-activity-7437597658095165440-Hy-G)). GitHub's creation date of Nov 2025 fits the latter, and the former likely describes the viral burst
- Among 4,400 Stack Overflow respondents answering on agent orchestration tools: LangChain 30.2%, OpenAI Agents SDK 23.8%, LangGraph 18.8%, Hermes Agent 10.2% — [Stack Overflow, AI data, Oct 2026](https://survey.stackoverflow.co/2026/ai/data)

### Inferences
- Ordering for individuals, with moderate confidence: coding agents are the only category with several consistent measures. Claude Code leads the developer surveys. Codex is rising fastest and may be close or ahead among consumers, though that rests on one survey. ChatGPT's agent features may reach the most people through distribution, but no data confirm this.
- The 39% against 65.5% gap for Claude Code reflects population and question, not error: JetBrains is reweighted and counts use at work, while Stack Overflow is self-selected and counts "used" among those answering. Stack Overflow's audience probably skews to heavier agent adopters. The trend is firmer than either level.
- Atlas's closure suggests the standalone-agent-browser format was hard to sustain, though OpenAI kept the capability inside ChatGPT. This is a product-format signal and not evidence on demand for browser agents.
- Stars measure attention rather than use. OpenClaw's stars rose while reported interest fell, so neither "collapse" nor "393K stars" is a reliable measure of active users.
- Disclosure: these notes were written by Claude, an Anthropic model, and several findings favour Anthropic's products. The rankings come from third-party data, but the report writer should weigh them with that in mind.

### Gaps
- No independent telemetry (panel or clickstream) comparing agent products was found.
- No agent-only active-user figure was found for ChatGPT agent mode, Dots, Gemini agent features, Copilot agent mode, Meta Muse or Manus. A reported steep decline in ChatGPT agent usage could not be verified; I found no source for it and it should not be used.
- No standalone usage figures for research agents (such as Deep Research products) were found.
- Comet and Codex user figures rest on low-quality aggregators, and should be replaced with primary sources if available.
- Windows of comparison differ (Feb to Sep 2026), so product rankings shown together are not strictly same-date.

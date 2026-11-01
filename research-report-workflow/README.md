# Research Report Workflow

Give Claude Code a topic. It asks what you need, researches it in depth, and hands back a cited report.

Type `/research <topic>` and the workflow does the rest.

## How it works

1. **Clarify:** Claude asks about scope, audience, what you want to know, and source preferences. Nothing is searched until you answer.
2. **Plan:** it shows the brief and the sub-questions, then waits for your go-ahead.
3. **Research:** parallel research agents do a deep dive and aim for 15+ sources, favoring primary ones.
4. **Report:** a dated Markdown report with citations, ending in key takeaways and next steps.
5. **Check:** every claim needs a citation, and every question you asked must be answered or marked unanswered.
6. **Publish:** an optional private web page of the report.

## What's in this repo

- `workflows/research-report.md`: the recipe in plain English. This is the only file you edit to change the behavior.
- `.claude/commands/research.md`: the `/research` command. It just points to the recipe.
- `output/`: finished reports.
- `research_notes/`: the raw notes behind each report.

## Example: State of AI agents, October 2026

A full run of the workflow on one topic.

- **Question:** what are individuals and creators using AI agents for, what works, what is overhyped, and where is it heading?
- **Report:** [output/2026-10-30-state-of-ai-agents-2026.md](output/2026-10-30-state-of-ai-agents-2026.md) (99 cited sources)
- **Notes:** [research_notes/State of AI agents 2026/](research_notes/State%20of%20AI%20agents%202026/), one file per research track

What a finished report looks like:
- Bottom line in 3-5 bullets
- One findings section per question, with a numbered citation on each bullet
- Evidence labels: Independent, Survey, Vendor claim, Forecast, Anecdote, Enterprise
- A section on where sources disagree
- Key takeaways and recommended next steps
- A numbered source list

## Use it yourself

1. Install [Claude Code](https://claude.com/claude-code) and open this folder in it.
2. Run `/research <your topic>`.
3. Answer the questions, approve the plan, and the report lands in `output/`.

## Limits

- A deep dive uses a lot of your Claude usage. Try a narrow topic first.
- Spot-check a few citations before you publish anything from a report. Some sources are search excerpts only, and the report marks them.
- Claude compiled the example report, so it carries the same disclosure as the report itself.

# web-research skill

A Claude skill that researches a request on the web (websites, Reddit, forums), cross-checks what it finds, and then builds whatever you asked for, with citations.

## What it does

- Plans the questions your request depends on
- Searches with several phrasings, and reads the actual pages instead of snippets
- Reads Reddit threads, with fallbacks when Reddit blocks the fetch
- Confirms key facts in 2+ sources and reports disagreements
- Delivers the finished result, followed by a Sources list and a "Gaps & uncertainty" section

## Install

**Claude Code**

```bash
git clone https://github.com/OwenTjandra/web-research-skill.git
cp -r web-research-skill/web-research ~/.claude/skills/
```

Then type `/web-research <your request>`, or just ask for something that needs research.

**claude.ai**

1. Zip the `web-research` folder (the folder itself, with `SKILL.md` inside).
2. Go to Settings → Capabilities → Skills and upload the zip.
3. Turn on web search in the chat's tools menu.

## Example

```
/web-research write a buying guide for budget mechanical keyboards under $80, using what Reddit recommends
```

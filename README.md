# Anti-Slop Writing

A system prompt that reduces bad AI writing patterns in LLM output. Add [`writing.md`](writing.md) to your Claude Code projects or copy into your system prompt. The output should read less like AI slop. I hope.

## What it does

The file contains 40+ rules organized into four sections:

- **Hard bans** (17 categories). This is puffery, symbolism without evidence, brochure tone, triad padding, synonym stuffing, engagement-bait openers, copula avoidance, trailing -ing phrases, vague attributions, and model-specific tells for both Claude and ChatGPT.
- **Required behaviors** (6 rules). Use mechanism verbs, add checkable details to claims, prefer concrete over abstract, use "is" and "are" freely.
- **Output contract**. State uncertainty directly, do not fill gaps with generic positive language.
- **Self-audit**. Scan output against all rules before producing the final answer.

## Sources

- [Wikipedia: Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing) — patterns identified by Wikipedia editors
- Kobak et al., "Delving into LLM-assisted writing," *Science Advances* (2025). 900 excess words, open dataset at [berenslab/llm-excess-vocab](https://github.com/berenslab/llm-excess-vocab)
- Geng & Trotta, "Human-LLM Coevolution," ACL (2025). How tells fade when publicly identified and new ones replace them
- Ethan Mollick, LinkedIn, March 2026. Engagement-bait phrases identified as "generic Claudisms". https://www.linkedin.com/posts/emollick_linkedin-should-let-us-all-mute-the-following-activity-7437596263673495552-YPkt
- Gemini 3.1 Pro Deep Research on 16.03.2026. https://gemini.google.com/share/1a62000695ed
- ChatGPT 5.4 Thinking Extended Thinking Deep Research 16.03.2026. https://chatgpt.com/share/69b7d0af-de48-800a-8850-bfda9ccd08d0
- Claude Opus 4.6 Extended Research with same prompt as the others 16.03.2026. But I can't share it since "Chats using advanced research can't be shared"

## Contributing

Open an issue or pull request. New rules should have a cited source such as a published style guide, an academic paper, a Wikipedia policy page, or an editorial standard with identifiable author and date. Unsourced opinions about what "sounds like AI" will also be considered!

## License

MIT, aka "do whatever you want with this".

## Author

[Marius Aure](https://github.com/MariusAure)

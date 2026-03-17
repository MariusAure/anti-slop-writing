# Anti-Slop Writing

A system prompt that reduces AI writing patterns in LLM output. Add [`writing.md`](writing.md) to your Claude Code projects or copy it into your system prompt. I hope the output reads less like AI slop.

## How to use it

1. Copy the contents of [`writing.md`](writing.md).
2. Paste it into your LLM's system prompt, custom instructions, or project context.
3. Write your prompt as normal.

Works with ChatGPT, Claude, Gemini, and local models. No installation, no dependencies.

## What it does

36 lines. Four sections.

- **Banned words.** 40+ puffery and filler words that LLMs overuse (pivotal, seamless, landscape, tapestry, leverage, etc.). Ban unless you have the data to justify them.
- **Banned patterns.** Symbolism without evidence, formulaic structures ("In conclusion..."), engagement bait ("here's the thing nobody is talking about"), synonym rotation, vague attributions ("experts argue"), copula avoidance ("serves as" instead of "is"), trailing -ing phrases, epistemic cowardice, formatting tells.
- **Required behaviors.** Precision-first claims, mechanism verbs, concrete over abstract, neutral tone, varied rhythm.
- **Self-audit.** Scan output against all rules before producing the final answer.

## Sources

- [Wikipedia: Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing)
- Kobak et al., "Delving into LLM-assisted writing," *Science Advances*, 2025. [Dataset](https://github.com/berenslab/llm-excess-vocab)
- Geng & Trotta, "Human-LLM Coevolution," ACL, 2025
- Reinhart et al., "Do LLMs Write Like Humans?" *PNAS*, 2025
- Walters & Wilder, "Fabrication and errors in LLM citations," *Scientific Reports*, 2023
- Ethan Mollick, ["Claudisms"](https://www.linkedin.com/posts/emollick_linkedin-should-let-us-all-mute-the-following-activity-7437596263673495552-YPkt), LinkedIn, March 2026
- Sam Kriss, *New York Times Magazine*, December 2025
- Orwell, "Politics and the English Language," 1946

Deep research inputs used to build the rules:
- [Gemini 3.1 Pro](https://gemini.google.com/share/1a62000695ed), 16 March 2026
- [ChatGPT 5.4](https://chatgpt.com/share/69b7d0af-de48-800a-8850-bfda9ccd08d0), 16 March 2026
- Claude Opus 4.6 (can't share advanced research chats), 16 March 2026

## Contributing

Open an issue or pull request. Anything that makes AI writing less bad is welcome. Citations to a source are preferred, but opinions about what "sounds like AI" will be considered too.

## License

MIT, aka "do whatever you want with this".

## Author

[Marius Aure](https://github.com/MariusAure)

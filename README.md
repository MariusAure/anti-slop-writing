# Anti-Slop Writing

An all-purpose diagnostic-and-revision prompt for LLM writing. Add [`writing.md`](writing.md) to a Claude Code project or copy it into a system prompt, custom instruction, or project context. It helps models make prose clear, accurate, and useful without turning every genre into the same flat "human" voice.

## How to use it

1. Copy [`writing.md`](writing.md).
2. Paste it into your LLM's system prompt, custom instructions, or project context.
3. Give the model a normal writing or editing request.

Works with ChatGPT, Claude, Gemini, and local models. No installation or dependencies.

## What it does

The prompt treats common AI tells as diagnostic signals, not universal bans. It asks the model to:

- start with the reader and the job to be done;
- use a concrete avoid list to find generic phrasing, vague abstraction, canned warmth, and unsupported intensity;
- test suspect sentences for meaning, fungibility, evidence, and genre fit;
- preserve uncertainty and factual scope, and flag hollow spans instead of inventing detail;
- use structure, voice, and punctuation when they help the requested form; and
- revise silently unless the user asks for an explanation or change log.

The result should be more specific and readable, not merely less detectable. A neutral support article and a personal essay have different jobs; the prompt makes room for both.

## Sources and design basis

- Steph Zinn, ["The habits of AI writing — and what to do about them"](https://a16zcrypto.substack.com/p/the-habits-of-ai-writing-and-what), a16z crypto, 2026
- Karen Rødland Thowsen and Dagne Omland, ["Slik avslører du en KI-generert tekst"](https://www.dn.no/d2/teknologi/kunstig-intelligens/sprak/sprakmodell/slik-avslorer-du-en-ki-generert-tekst/2-1-2021015), DN/D2, 24 September 2026 -- unnecessary contrasts, Norwegian word choice, and literal translations from English.
- [OpenAI model guidance: prompting best practices](https://developers.openai.com/api/docs/guides/latest-model) -- keep prompts lean, state requirements once, and evaluate representative tasks.
- [Anthropic prompting best practices](https://platform.claude.com/docs/en/build-with-claude/prompt-engineering/claude-prompting-best-practices) -- provide clear task context and use relevant, diverse examples for reliable style control.
- [Agent Skills best practices](https://agentskills.io/skill-creation/best-practices) -- include only high-signal instructions and refine them through real execution.
- [de-slop](https://github.com/isatimur/de-slop) -- fidelity-first editing: identify hollow spans and do not fabricate details to improve them.
- [Wikipedia: Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing)
- Kobak et al., "Delving into LLM-assisted writing," *Science Advances*, 2025. [Dataset](https://github.com/berenslab/llm-excess-vocab)
- Geng & Trotta, "Human-LLM Coevolution," ACL, 2025
- Reinhart et al., "Do LLMs Write Like Humans?" *PNAS*, 2025
- Walters & Wilder, "Fabrication and errors in LLM citations," *Scientific Reports*, 2023
- Orwell, "Politics and the English Language," 1946
- Thomas & Turner, *Clear and Simple as the Truth*, 2011
- Pinker, *The Sense of Style*, 2014

## Contributing

Open an issue or pull request. Prefer changes supported by a source or a repeatable before-and-after example. The standard is better writing for a real reader, not a longer list of things that look like AI.

## License

MIT, aka "do whatever you want with this".

## Author

[Marius Aure](https://github.com/MariusAure)

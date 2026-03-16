# Anti-Slop Writing

A system prompt that reduces AI writing patterns in LLM output. One file. Copy it into your system prompt. The output reads less like a machine wrote it.

## How to use it

1. Copy the contents of [`writing.md`](writing.md).
2. Paste it into your LLM's system prompt, custom instructions, or project context.
3. Write your prompt as normal.

Works with ChatGPT, Claude, Gemini, and local models. No installation, no dependencies.

## What it does

The file contains 40+ rules organized into four sections:

- **Hard bans** (17 categories): puffery, symbolism without evidence, brochure tone, triad padding, synonym stuffing, engagement-bait openers, copula avoidance, trailing -ing phrases, vague attributions, and model-specific tells for both Claude and ChatGPT.
- **Required behaviors** (6 rules): use mechanism verbs, add checkable details to claims, prefer concrete over abstract, use "is" and "are" freely.
- **Output contract**: state uncertainty directly, do not fill gaps with generic positive language.
- **Self-audit**: scan output against all rules before producing the final answer.

## Why "slop"

"Slop" is the term for low-quality AI-generated content that sounds fluent but says little. Kobak et al. (Science Advances, 2025) analyzed 15 million PubMed abstracts and found 900 words used at abnormal frequency in post-ChatGPT papers. "Delve" appeared at 25x expected frequency. At least 200,000 academic papers per year showed signs of LLM processing. This prompt targets those patterns at the source.

## Sources

Every rule cites its origin. The primary sources:

- [Wikipedia: Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing) — patterns identified by Wikipedia editors
- Kobak et al., "Delving into LLM-assisted writing," *Science Advances* (2025) — 900 excess words, open dataset at [berenslab/llm-excess-vocab](https://github.com/berenslab/llm-excess-vocab)
- Geng & Trotta, "Human-LLM Coevolution," ACL (2025) — how tells fade when publicly identified and new ones replace them
- Ethan Mollick (Wharton), LinkedIn, March 2026 — engagement-bait phrases identified as "generic Claudisms"
- Orwell, "Politics and the English Language" (1946)
- Strunk & White, "The Elements of Style"

## Contributing

Open an issue or pull request. New rules require a cited source: a published style guide, an academic paper, a Wikipedia policy page, or an editorial standard with identifiable author and date. Unsourced opinions about what "sounds like AI" are not sufficient.

## License

MIT

## Author

[Marius Aure](https://github.com/MariusAure)

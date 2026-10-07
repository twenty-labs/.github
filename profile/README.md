# Twenty Labs

Twenty Labs is an AI-focused technology company building practical products that help people learn, work, and communicate more effectively.

We focus on solving one problem completely before moving on to the next. Below are the tools we build for our own work and publish for anyone to use.

## Open tools

| Tool | What it does | Install |
| --- | --- | --- |
| [**AI OS**](https://www.npmjs.com/package/@twentylabs/ai-os) | CLI that compiles one company-wide definition of how AI agents work (roles, skills, policies, knowledge) into any repository, for the AI runtimes people use: Claude Code, Codex, Cursor, Claude Desktop and ChatGPT. | `npx -y @twentylabs/ai-os init --registry-version <version>` |
| [**AI OS registry**](https://www.npmjs.com/package/@twentylabs/ai-os-registry) | The content behind AI OS: roles, skills, policies, knowledge slots and profiles. Data only, versioned with semver. | Pinned in each repository's `ai-os.yaml` |
| [**AI OS marketplace**](https://github.com/twenty-labs/ai-os-marketplace) | Claude Code plugin marketplace generated from the registry: one plugin per role and per skill. | `/plugin marketplace add twenty-labs/ai-os-marketplace` |
| [**gads**](https://www.npmjs.com/package/@twentylabs/gads) | Scriptable CLI for the Google Ads API: profiles, GAQL queries, and validated change files. | `npm i -g @twentylabs/gads` |
| [**asa**](https://www.npmjs.com/package/@twentylabs/asa) | Apple Ads from the terminal, on top of the open-source `asc` CLI: read-only report pulls and approved change files. | `npm i -g @twentylabs/asa` |

All npm packages are MIT licensed.

## How we work

- **Open standards first.** `AGENTS.md` is the shared instruction file and belongs to the project; skills follow the Agent Skills `SKILL.md` standard.
- **English instructions, any conversation language.** Skills, personas and policies are written in English; agents answer in the language you use.
- **Exact pins, no silent drift.** Each repository pins the exact CLI and registry versions it uses; CI fails when generated files drift, and upgrades summarize what changed.
- **Humans approve changes.** Our ad tools validate or preview by default and only write with an explicit `--yes`, saving the state before and after as evidence.

## Contact

- Website: [thetwentylabs.com](https://thetwentylabs.com/)
- Email: [contact@thetwentylabs.com](mailto:contact@thetwentylabs.com)

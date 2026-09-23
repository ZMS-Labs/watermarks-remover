# Fork guide

This is my fork of [guillaumemeyer/watermarks-remover](https://github.com/guillaumemeyer/watermarks-remover), archived as a read-only copy of upstream v0.3.0. The skill and scripts come from the upstream project, and its MIT license still applies. The changes here are documentation only.

Use the tool only on files you own or are allowed to process, and keep your originals. A cleaned file doesn't give you legal permission or anonymity, and it can still carry signs of where it came from that the tool doesn't reach. Upstream's [ethics notes](skills/remove-ai-marks/references/ethics.md) list what the tool is and isn't for.

## Start here

| Task | Where to look |
|---|---|
| See what the tool does with text and files | [README](README.md) |
| Read the agent skill | [Skill instructions](skills/remove-ai-marks/SKILL.md) |
| Ask about or change the tool | [The upstream project](https://github.com/guillaumemeyer/watermarks-remover) |
| Report a potential vulnerability | [Security policy](SECURITY.md) |
| Check reuse terms | [MIT license](LICENSE) |

Issues are off here, and the badges and release links in the README point to upstream. If the fork is ever updated, upstream's credits and MIT license stay as they are.

## Run the tests

The core scripts need only Python's standard library. The [tests](tests) use pytest. With it installed, `python -m pytest` runs the suite, the same as `make test` in the [Makefile](Makefile).

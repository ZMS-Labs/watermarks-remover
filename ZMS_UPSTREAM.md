# Fork guide

This repository is a ZMS Labs fork of [guillaumemeyer/watermarks-remover](https://github.com/guillaumemeyer/watermarks-remover). The upstream project supplies the skill and scripts described in the [README](README.md). This guide distinguishes the fork from upstream without changing the upstream license or product claims.

## Start here

| Task | Guide or source |
|---|---|
| Understand supported text and file operations | [README](README.md) |
| Read the agent skill | [Skill instructions](skills/remove-ai-marks/SKILL.md) |
| Find verification commands | [Makefile](Makefile) and [tests](tests) |
| Propose a change | [Contribution guide](CONTRIBUTING.md) |
| Report a potential vulnerability | [Security policy](SECURITY.md) |
| Check reuse conditions | [MIT license](LICENSE) |

The inherited contribution guide describes upstream maintainers and branch protection; it does not establish this fork's permissions or protection settings.

Upstream badges, releases, and support links describe upstream. They do not prove that the fork has published an equivalent release or passed the same checks. Inspect this repository's commits and check results for a fork-specific claim.

## Verify and contribute

Core scripts use the standard library; the test suite uses pytest. With the test dependencies available, `python -m pytest` runs the repository suite, matching `make test`. The Makefile also defines smoke checks and optional integrations. Optional model or external-tool checks should be run only with the intended configuration and authorization.

Use synthetic fixtures or content you are authorized to process. Preserve originals when evaluating file transformations. A transformation result does not establish legal permission, anonymity, or the absence of every possible provenance signal.

Route upstream product changes to the upstream project. Use this fork's issue tracker for a fork-specific regression, and identify the relevant commit or local difference. Preserve upstream authorship and licensing when updating the fork.

## Visual documentation quality

Apply the [shared visual documentation standard](https://github.com/ZMS-Labs/.github/blob/main/docs/documentation-standard.md#use-visuals-to-explain)
to all new or changed visual headings, Mermaid diagrams, flowcharts, sequences,
screenshots, and charts. Verify labels, arrows, grouping, order, and status
against authoritative source; distinguish conceptual, planned, implemented, and
observed evidence. Preserve authentic product screenshots and product-local
design identity. Use generated images only for illustrative explanation, and
keep exact diagrams editable.

Inspect the rendered destination at desktop and narrow widths, with readable
labels, a text equivalent, and light/dark presentation where supported. Record
the source scope, actual semantic and render checks, and remaining limits in the
change description. Use one bounded review and recheck affected content; this
standard adds no mandatory independent-model gate. Adoption does not certify
that historical visuals have been reviewed.

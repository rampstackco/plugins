# RampStack plugins

The Claude Code plugin marketplace for the [RampStack](https://github.com/rampstackco/claude-skills) skill catalog. One place to add, then install any of the curated RampStack skill plugins.

## Install

Add this marketplace once, then install whichever subset you want:

```
/plugin marketplace add rampstackco/plugins
/plugin install rampstack-starter@rampstack
```

The other two plugins install the same way:

```
/plugin install rampstack-seo@rampstack
/plugin install rampstack-pm@rampstack
```

## Plugins

| Plugin | What it covers | Skills | Source repo |
|---|---|---|---|
| `rampstack-starter` | A general-purpose subset across the website lifecycle: code review, QA, performance, frontend, design, content, SEO, conversion, and product specs | 14 | [rampstackco/claude-skills-starter](https://github.com/rampstackco/claude-skills-starter) |
| `rampstack-seo` | SEO operations: keyword research, on-page and technical audits, AI-search optimization, traffic diagnosis, site-health triage, competitor and content audits, programmatic SEO, plus content companions | 12 | [rampstackco/claude-skills-seo](https://github.com/rampstackco/claude-skills-seo) |
| `rampstack-pm` | Product management across the lifecycle: discovery, roadmaps and OKRs, PRDs, stakeholder communication, launches, beta programs, and measurement | 12 | [rampstackco/claude-skills-pm](https://github.com/rampstackco/claude-skills-pm) |

The `rampstack-seo` plugin includes a handful of skills that assume the Ahrefs MCP for the deep-audit workflows. The rest of the SEO skills work without it.

## Trust

The plugins listed here install skill files only. A skill is a markdown `SKILL.md` plus its reference material. Installing one of these plugins copies that content into your Claude Code plugin cache so Claude can read it. The plugin payload does not include or run executable code, hooks, or MCP servers.

The plugin source repos do contain an author-time social-card generation script under `tools/` with a Playwright dev dependency. That script is run manually by the maintainers to regenerate the GitHub social preview image, is not packaged into the plugin, and does not run on install.

## Catalog

This marketplace lists curated subsets. The full RampStack skill catalog (102 skills, the source of truth for all skill content) lives at [rampstackco/claude-skills](https://github.com/rampstackco/claude-skills). The starter, SEO, and PM plugins are subsets of that catalog with no modifications to skill content.

## Related repos

- [claude-skills](https://github.com/rampstackco/claude-skills): the full catalog.
- [claude-skills-starter](https://github.com/rampstackco/claude-skills-starter): the starter plugin source.
- [claude-skills-seo](https://github.com/rampstackco/claude-skills-seo): the SEO plugin source.
- [claude-skills-pm](https://github.com/rampstackco/claude-skills-pm): the PM plugin source.

## License

MIT. See [LICENSE](LICENSE).

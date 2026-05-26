# Security Policy

## Reporting a vulnerability

If you discover a security vulnerability in this repository, please report it privately. Do **not** open a public GitHub issue.

### Preferred: GitHub Security Advisories

The fastest way to report is via GitHub's private vulnerability reporting:

1. Go to the [Security tab](https://github.com/rampstackco/plugins/security) of this repository
2. Click **Report a vulnerability**
3. Fill out the form with as much detail as possible

This keeps the report confidential while we investigate.

### Alternate: email

You can also email the security team directly at **security@rampstack.co**.

When reporting, please include:

- A description of the vulnerability
- Steps to reproduce
- The potential impact
- Any suggested mitigation, if you have one
- Whether you would like public credit when the fix ships

## What to expect

- **Acknowledgment** within 3 business days
- **Initial assessment** within 7 business days, including a severity classification
- **Status updates** every 7 days while the fix is in progress
- **Public disclosure** coordinated with the reporter once a fix is available

## Scope

This repository is a Claude Code plugin marketplace. The only files it ships are the marketplace manifest (`.claude-plugin/marketplace.json`), the marketplace documentation, and the validation workflow. The most likely security concerns here are:

- **Marketplace manifest tampering** that would redirect a plugin source to an unintended repository
- **Misleading documentation** that could lead a user to install an unintended plugin or marketplace
- **CI workflow vulnerabilities** in the manifest validation pipeline

## Out of scope

The following are not security vulnerabilities for this repository:

- Issues with the skill content itself. Skill content lives in the source catalog at [rampstackco/claude-skills](https://github.com/rampstackco/claude-skills); report those there.
- Issues with an individual plugin's source repository. Report those to the corresponding plugin repo: [claude-skills-starter](https://github.com/rampstackco/claude-skills-starter), [claude-skills-seo](https://github.com/rampstackco/claude-skills-seo), or [claude-skills-pm](https://github.com/rampstackco/claude-skills-pm).
- Issues with how Claude itself handles plugins. Report those to [Anthropic](https://www.anthropic.com/security).
- Issues with third-party tools recommended in any skill (Ahrefs MCP, GitHub MCP, etc.). Report those to the respective vendors.
- General feedback or suggestions on plugin packaging. Use [Issues](https://github.com/rampstackco/plugins/issues) for those.

## Hall of fame

We thank security researchers who responsibly disclose vulnerabilities. With permission, we will list contributors who help keep this repository safe in this section.

_No reports yet._

---

Thank you for helping keep this project and its users safe.

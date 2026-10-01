# CRM Launch Operator

**Launch a CRM your team can use—and reports you can trust.**

A new CRM can get expensive fast when nobody is quite sure how it should be set up, what belongs in it, or whether the reports are telling the truth. CRM Launch Operator Lite is a free, open-source AI skill that helps a business owner get clear before setup choices multiply.

It runs a calm, roughly ten-minute **CRM Launch Check** and creates one local file covering:

- what you want the CRM to fix;
- who needs to use it;
- the minimum rule for what belongs;
- the three biggest unanswered decisions;
- an `Owned / Moving / Trusted` check;
- a plain conclusion; and
- the next useful action.

It does not log into or operate your CRM. Your answers stay in the workspace where you run the skill.

## Install Lite

Lite is available as a Codex Git marketplace plugin and as a standalone skill
ZIP for Codex, Claude, and other compatible skill hosts. Lite has no network
tools, CRM connection, or automatic support workflow. The public OpenAI plugin
directory listing is pending.

### Codex plugin

In Codex CLI, install the public Git marketplace plugin:

```sh
codex plugin marketplace add https://github.com/mikeeads/crm-launch-operator.git
codex plugin add crm-launch-operator-lite@crm-launch-operator
```

Version 1.2.0 was verified with Codex CLI `0.159.2` and `gpt-6.1-sol`, including
a fresh start, saved answer, and fresh resume. Earlier `gpt-5.6-sol` marketplace
runs failed to read the installed skill; use the standalone ZIP if that route
does not load the skill in your host.

Start a new thread so Codex picks up the installed skill, then say:

> Use $crm-launch-operator-lite to run a calm CRM Launch Check with me, one question at a time.

If Codex says the skill instructions are unavailable or no
`crm-launch-check.md` file appears, the activation failed.
A plausible question without that file is not activation.

### Codex

Download the versioned ZIP and `SHA256SUMS` from the [latest GitHub release](https://github.com/mikeeads/crm-launch-operator/releases/latest), verify the checksum if your tool supports it, unzip it once, and place the whole `crm-launch-operator-lite` folder in your personal skills directory (normally `~/.agents/skills/`). Restart Codex if the skill is not picked up immediately.

Then start with:

> Use $crm-launch-operator-lite to run a calm CRM Launch Check with me, one question at a time.

[Codex skills documentation](https://developers.openai.com/codex/skills)

### Claude

Download the versioned ZIP from the [latest GitHub release](https://github.com/mikeeads/crm-launch-operator/releases/latest) and upload it as a custom skill in Claude without unzipping it. Then ask Claude to use CRM Launch Operator Lite for a CRM Launch Check.

[Claude custom skills help](https://support.claude.com/en/articles/12512180-use-skills-in-claude)

## Want the full edition?

Launching HubSpot or Pipedrive? There is a fuller version with platform-specific guidance, launch files, local checks, team testing, and a private home base. **Every edition is free.**

[Ask for the free full edition](https://crm.coach/launch-operator)

Lite is useful on its own. The full edition is there when you want to work through the implementation and reach a clear launch decision.

## Safety and privacy

- Do not give an AI passwords, API keys, session cookies, or recovery codes.
- Use sanitized sample records instead of unnecessary personal customer data.
- The skill advises; it does not make CRM changes or approve a launch for you.
- Review any third-party AI product's privacy and data controls before using business information.

## License

The code and skill instructions in this repository are licensed under the [Apache License 2.0](LICENSE). The CRM Coach and CRM Launch Operator names and branding are not granted under that license; see [TRADEMARKS.md](TRADEMARKS.md).

See [PRIVACY.md](PRIVACY.md), [TERMS.md](TERMS.md), [SUPPORT.md](SUPPORT.md), and [CONTRIBUTING.md](CONTRIBUTING.md) for the boundaries around using and improving the public skill.

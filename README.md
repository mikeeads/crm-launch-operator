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

### Codex

Download the latest ZIP from `releases/`, unzip it, and place the `crm-launch-operator-lite` folder in your user skills directory (normally `~/.agents/skills/`). Restart Codex if the skill is not picked up immediately.

Then start with:

> Use $crm-launch-operator-lite to run a calm CRM Launch Check with me, one question at a time.

[Codex skills documentation](https://developers.openai.com/codex/skills)

### Claude

Download the latest ZIP from `releases/` and upload it as a custom skill in Claude. Then ask Claude to use CRM Launch Operator Lite for a CRM Launch Check.

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

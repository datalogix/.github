# .github

Organization-wide defaults and settings for `datalogix` repositories. GitHub applies the issue forms and `FUNDING.yml` only to repositories without their own.

- `.github/ISSUE_TEMPLATE/`: issue forms that hand an issue to Claude. They only work in projects set up with the Claude workflows and labels (`claude`, `claude-plan`): elsewhere the issue opens and nothing runs.
- `.github/FUNDING.yml`: the default Sponsor button, shown only in repositories with Sponsorships turned on in their settings.
- `workflows/relay.json`: the monitoring relay's settings, read by each project's setup.

The issue forms and `relay.json` are generated: the organization's setup overwrites the forms on each run and `relay.json` when it updates the relay, so edits made here are lost.

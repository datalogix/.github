# .github

Organization-wide defaults and settings for `datalogix` repositories. GitHub applies the issue forms and `FUNDING.yml` only to repositories without their own.

- `.github/ISSUE_TEMPLATE/`: issue forms that hand an issue to Claude. They only work in repositories that have their labels (`claude`, `claude-plan`): GitHub does not create a missing label, so the issue opens without it and nothing runs.
- `.github/FUNDING.yml`: the default Sponsor button.
- `workflows/relay.json`: the monitoring relay's settings, read by each project's setup.

The [`org` command](https://github.com/datalogix/workflows/blob/v2/docs/organization-setup.md) of `datalogix/workflows` writes the issue forms and `relay.json`, and overwrites the forms on each run: change them there, not here.

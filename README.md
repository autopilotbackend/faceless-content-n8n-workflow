# Faceless Content Workflows for n8n

Three free n8n workflows for running a faceless content pipeline on your own server.

| File | What it does |
|---|---|
| `workflows/01-research-workflow.json` | Every morning, pulls fresh topic ideas from Reddit and YouTube, scores them with Claude, and adds the best ones to a Google Sheet. |
| `workflows/00-error-alerts.json` | Emails you when any workflow fails, with a plain-English hint about what broke. |
| `workflows/05-weekly-numbers-report.json` | Every Monday, emails a short summary of what you published that week. |

## How to use one

1. In n8n, open Workflows, click the three dots, then Import from File.
2. Pick one of the files in the `workflows` folder.
3. Add your own credentials to the nodes that need them (Google Sheets, email, Anthropic).
4. Replace `you@example.com` and the sheet placeholder with your own values.
5. Turn it on.

No logins or keys are stored in these files. You add your own.

## Want the whole system?

This repo has 3 of the 15 workflows we run. The free research workflow comes with a short email series at **[get.autopilotbackend.com](https://get.autopilotbackend.com)**. The full pack covers research, scripts, voice, video, publishing, and reports.

## No server yet?

Deploy n8n with a Postgres database on Railway in one click, then import the files above: **[Deploy on Railway](https://railway.com/deploy/autopilot-backend-n8n)**. The Dockerfile, `railway.json` and `.env.example` in this repo are what the template uses.

## License

MIT. Use it, change it, share it.

Built by [Autopilot Backend](https://get.autopilotbackend.com).

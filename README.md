# Talent Intelligence

AI-powered HR excellence platform - Your Fractional CHRO.

## Features

- **Talent Assessment**: 9-box grids, performance & potential analysis
- **Retention Analytics**: Flight risk prediction, retention strategies
- **Workforce Planning**: Headcount forecasting, skill gap analysis
- **Succession Planning**: Leadership pipeline, bench strength
- **Diversity & Inclusion**: Representation metrics, pay equity analysis
- **AI Consultation**: Claude-powered CHRO consultant

## Tech Stack

- **Backend**: Flask, SQLAlchemy, PostgreSQL
- **AI**: Anthropic Claude API
- **Frontend**: Bootstrap 5
- **Deployment**: Render

## Quick Start

```bash
pip install -r requirements.txt
export ANTHROPIC_API_KEY=$(az keyvault secret show --vault-name kv-demo-apps-shared --name Demo-Apps-Share-API-Key --subscription "Demo Apps" --query value -o tsv)
python web/app.py
```

## LLM API key

The Anthropic API key is optional: without it the app runs but the AI consultant reports that it is unavailable. The key is the shared secret `Demo-Apps-Share-API-Key` in Azure Key Vault `kv-demo-apps-shared` (subscription "Demo Apps"). Fetch it with:

```bash
az keyvault secret show --vault-name kv-demo-apps-shared --name Demo-Apps-Share-API-Key --subscription "Demo Apps" --query value -o tsv
```

Set the result as `ANTHROPIC_API_KEY` (on Render, in the dashboard). The model is `claude-sonnet-5-5` (Claude Sonnet 5.5).

## Part of Fractional C-Suite

- **CFO**: Cash Flow Intelligence
- **CTO**: App Rationalization Pro
- **COO**: Operations Intelligence
- **CHRO**: Talent Intelligence (this project)

## License

Proprietary - Patriot Tech Systems Consulting LLC

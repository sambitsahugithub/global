# AI Learning Hub

A comprehensive, single-source AI learning portal covering Microsoft and AWS platforms — from first prompt to enterprise agentic systems. GCP coming next.

## What's inside

| Section | Content |
|---|---|
| AI Tools Overview | 6 tools compared (ChatGPT, Claude, Gemini, Copilot, Perplexity, GitHub Copilot) + when-to-use guide |
| Microsoft Platform | Copilot, Copilot Studio, Azure OpenAI, AI Foundry, AI Search, Semantic Kernel |
| Microsoft Learning Paths | 3 tracks: AI Foundations → AI Builder → AI Architect |
| Microsoft Curriculum | 16 filterable modules with Theory / Practical / Lab tags |
| Microsoft Labs | 6 hands-on labs (FAQ agent → Multi-agent orchestration) |
| Microsoft Resources | 6 curated official links |
| AWS Platform | Bedrock, AgentCore, Knowledge Bases, SageMaker, Amazon Q, Guardrails, Flows |
| AWS Learning Paths | 3 tracks: Practitioner → Associate → Professional |
| AWS Curriculum | 16 filterable modules covering all Bedrock and SageMaker topics |
| AWS Labs | 6 hands-on labs (first chatbot → multi-agent system) |
| AWS Resources | 6 curated official links including Skill Builder and Workshops |
| Certifications | 10 certs mapped across MS and AWS with tabs, retirement warnings |
| 6-Month Roadmap | Combined MS + AWS learning journey with certification milestones |
| FAQ | 6 common questions answered |
| Azure Deploy | Static Web App deployment instructions |

## Navigation structure

```
Top Nav
├── Overview        (AI Tools landscape — standalone)
├── AI Tools        (comparative overview — standalone)
├── Microsoft ▼     (dropdown group)
│   ├── Platform Overview
│   ├── Learning Paths
│   ├── Curriculum
│   ├── Labs
│   └── Resources
├── AWS ▼           (dropdown group)
│   ├── Platform Overview
│   ├── Learning Paths
│   ├── Curriculum
│   ├── Labs
│   └── Resources
├── Certifications  (all platforms — standalone)
└── Roadmap         (6-month journey — standalone)
```

## Deploy to Azure Static Web Apps

```bash
az group create --name rg-ai-hub --location eastus2

az staticwebapp create \
  --name ai-learning-hub \
  --resource-group rg-ai-hub \
  --source https://github.com/YOUR-ORG/ai-learning-hub \
  --location eastus2 \
  --branch main \
  --app-location "/" \
  --sku Free
```

## Files

| File | Purpose |
|---|---|
| `index.html` | Complete single-file portal |
| `staticwebapp.config.json` | Azure SWA routing + security headers |
| `.github/workflows/azure-static-web-apps.yml` | CI/CD pipeline |
| `README.md` | This file |

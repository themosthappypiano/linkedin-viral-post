# LinkedIn Content Research Workflow

A lightweight interface for launching LinkedIn content-research jobs through an n8n automation workflow.

Users can select a niche, generate or add keywords, configure search criteria, preview the request, and send it to the connected n8n webhook for processing.

## Features

- Niche-based keyword generation
- Custom keyword selection
- Search and engagement filters
- Request preview before submission
- n8n webhook integration
- Responsive single-page interface
- Express health endpoint for deployment monitoring

## Technology

- HTML, CSS, and vanilla JavaScript
- Node.js and Express
- n8n for workflow orchestration
- Render deployment configuration

## Local development

Requirements: Node.js 18 or newer.

```bash
npm install
npm start
```

Open [http://localhost:3000](http://localhost:3000). The health endpoint is available at `/health`.

## How it works

1. The user selects a niche or adds custom keywords.
2. The interface prepares the research parameters.
3. The request is sent to an n8n webhook.
4. The external workflow performs the collection and analysis steps.

The repository contains the interface and webhook handoff. The downstream n8n workflow is managed separately.

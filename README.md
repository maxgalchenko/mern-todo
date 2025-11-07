# MERN Todo

<div align="center">

<img alt="React" src="https://img.shields.io/badge/React-17-61DAFB?logo=react&logoColor=white" />
<img alt="Create React App" src="https://img.shields.io/badge/CRA-4.0.1-09D3AC?logo=create-react-app&logoColor=white" />
<img alt="Node.js" src="https://img.shields.io/badge/Node.js-18-339933?logo=nodedotjs&logoColor=white" />
<img alt="Express" src="https://img.shields.io/badge/Express-4-black?logo=express&logoColor=white" />
<img alt="Elasticsearch" src="https://img.shields.io/badge/Elasticsearch-7-005571?logo=elasticsearch&logoColor=white" />
<img alt="Docker" src="https://img.shields.io/badge/Docker-Compose-2496ED?logo=docker&logoColor=white" />

</div>

## Overview

Simple full‑stack todo app demonstrating CRUD and search with an Express API backed by Elasticsearch. The React client (CRA) interacts with REST endpoints to manage todos and perform match‑based search. Docker Compose is provided to run Elasticsearch and Kibana locally.

## Key Features

- CRUD todos via REST API
- Full‑text search by name using Elasticsearch
- Inline edit and delete interactions in the list

## Tech Stack

React 17 (Create React App), Node.js 18, Express 4, Elasticsearch 7, Docker Compose

## Architecture

CRA frontend consuming an Express REST API. Elasticsearch is used as the primary datastore and search engine (no ORM). Local component state manages UI; `docker-compose.yml` provisions Elasticsearch and Kibana for local development.

## Performance & Accessibility

Lightweight client via CRA defaults; simple views with semantic HTML. Inline editing supports keyboard submit (Enter) and blur to save.

## Quality

- Linting: CRA ESLint presets • Formatting: not configured
- Type safety: none
- Tests: CRA test runner available; no tests present
- CI: not configured

## Prerequisites

- Node.js: `18.17.0`
- Docker (optional): to run Elasticsearch + Kibana locally

## Installation

```bash
git clone https://github.com/maxgalchenko/mern-todo.git
cd mern-todo
npm install
cd backend && npm install
```

## Quick Start

```bash
# Terminal 1 - client
npm start

# Terminal 2 - API
cd backend && npm run dev

# Production (client build)
cd .. && npm run build
# API production
cd backend && npm start
```

Open http://localhost:3000

## Available Scripts

- `npm start` – start CRA dev server (client)
- `npm run build` – build client for production
- `npm test` – run CRA test runner (no tests included)
- `cd backend && npm run dev` – start API with nodemon
- `cd backend && npm start` – start API in production mode

---

<div align="center">

Built with ❤️ by [Maksym Galchenko](https://github.com/maxgalchenko)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/galchenko-max/)
[![Portfolio](https://img.shields.io/badge/Portfolio-Visit-green?style=for-the-badge&logo=web)](https://portfolio-green-six-29.vercel.app/)
[![Email](https://img.shields.io/badge/Email-Contact-red?style=for-the-badge&logo=gmail)](mailto:galchenko.maksym@gmail.com)
![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)

</div>

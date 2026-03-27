# Basic Documentation

Welcome to the official documentation for Basic, a local-first database designed for user-owned data.

## Maintaining `openapi.json`

The file [`openapi.json`](./openapi.json) should stay in sync with the deployed Admin API. Regenerate it from the live spec (same host as the docs playground):

```bash
curl -sS 'https://api.basic.tech/docs/json' -o openapi.json
# optional: pretty-print
python3 -c "import json; p='openapi.json'; d=json.load(open(p)); json.dump(d, open(p,'w'), indent=2)"
```

When developing against a local admin server, substitute your local base URL and `/docs/json`.

## 🚀 Quick Start

To get started with Basic:

1. [What is Basic?](https://docs.basic.tech/get-started/welcome) and [Admin & project setup](https://docs.basic.tech/get-started/adminportal)
2. Pick an integration guide:
   - [React](https://docs.basic.tech/basic-react/basic-react-sdk)
   - [Next.js](https://docs.basic.tech/basic-nextjs/basic-nextjs-sdk)
   - [REST API](https://docs.basic.tech/basic-restapi/basic-api)

## 🌟 Key Features

- User-owned Personal Data Stores (PDS)
- Local-first sync for offline support and real-time capabilities
- OAuth 2.0 authentication included

## 📚 Core Concepts

- [Personal data stores](https://docs.basic.tech/readings/personal-data-stores)
- [Local-first sync](https://docs.basic.tech/readings/local-first-sync)
- [Basic Auth (OAuth)](https://docs.basic.tech/readings/auth-basic)
- [Managing permissions](https://docs.basic.tech/readings/permissioning)

## 🛠 API reference

- [Auth APIs](https://docs.basic.tech/api-reference/auth/redirect-to-sign-in)
- [Management APIs](https://docs.basic.tech/api-reference/projects/create-a-new-project) (projects, users, teams, keys)

## 💻 SDK reference

- [React hooks & provider](https://docs.basic.tech/sdk-reference/react-hooks)

## 🗺 Roadmap

See the [roadmap](https://docs.basic.tech/readings/others/roadmap).

## 🤝 Connect with Us

- [Twitter](https://twitter.com/basic_db)
- [GitHub](https://github.com/basicdb)
- [Book a Call](https://cal.com/basic/30min?user=basic&date=2024-09-20&month=2024-09)

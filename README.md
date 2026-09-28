# QATS Trader API

Public documentation for QATS account-bound trading connections.

**[Open the documentation](https://quantityproject.github.io/qats-trader-api/)**

Market data, account risk, orders, executions, positions and command recovery. Includes Python, JavaScript and cURL examples, OpenAPI and a Postman collection.

This repository contains documentation only. Trading keys, backend code and customer records are not included. API tokens are created on QATS, never on this GitHub Pages site. QATS uses its own Bearer-token protocol; Binance and Bybit clients are not wire-compatible.

## Local preview

Node 24+: `npm install`, then `npm run dev`. Build: `npm run build`.

## Publication

The `docs/` folder is the reviewed static build served by GitHub Pages. Changes to documentation sources must be rebuilt before publishing. Do not commit credentials or populated Postman variables.

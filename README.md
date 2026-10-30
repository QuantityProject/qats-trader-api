# QATS Trader API

Public documentation for the QATS Trader API: the REST API that lets a trader's own bot, script or TradingView strategy trade a [QATS Prop](https://prop.qats.us) account.

**[Open the documentation](https://quantityproject.github.io/qats-trader-api/)** · [QATS Prop](https://prop.qats.us) · [Free API sandbox](https://prop.qats.us/help/api-sandbox) · [Bots on QATS](https://prop.qats.us/help/bots)

Market data, account risk, orders, executions, positions and command recovery. Includes Python, JavaScript and cURL examples, OpenAPI and a Postman collection.

## What you can build

- **Trading bots** in Python, JavaScript or any language that speaks HTTPS, on crypto and TradFi USDT perpetuals priced from Binance and Bybit market data.
- **TradingView automation**: alerts and Pine strategies sent as webhooks to the same order routes (see [TradingView webhook alert JSON](https://prop.qats.us/blog/tradingview-webhook-alert-json)).
- **Your own tools** around a prop account: journals, risk dashboards, position sizing and reconciliation.

Every API order passes the same server-side risk checks as an order placed by hand in the QATS Trader terminal, so a bot cannot take an account past its loss limits by accident. Writes take an `Idempotency-Key`, and an uncertain result is confirmed by command ID instead of being resent.

## Start in the sandbox

The sandbox is free for every registered, verified QATS trader: a virtual $100,000 account with its own `qats_sandbox_` keys, separate from any purchased evaluation. Sandbox orders never reach an exchange. Create keys under Sandbox → Keys & connections, then follow [your first API order](https://prop.qats.us/help/api-first-order).

## About this repository

This repository contains documentation only. Trading keys, backend code and customer records are not included. API tokens are created on QATS, never on this GitHub Pages site. QATS uses its own Bearer-token protocol; Binance and Bybit clients are not wire-compatible.

QATS Prop evaluations and initial funded accounts operate in a simulated environment. Trading involves substantial risk.

## Local preview

Node 24+: `npm install`, then `npm run dev`. Build: `npm run build`.

## Publication

The `docs/` folder is the reviewed static build served by GitHub Pages. Changes to documentation sources must be rebuilt before publishing. Do not commit credentials or populated Postman variables.

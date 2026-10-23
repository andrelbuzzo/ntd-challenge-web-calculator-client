# NTD Web Calculator Client

React 19 single-page client for the NTD arithmetic calculator. The client authenticates against the Spring Boot API and provides calculator, balance, and records/history flows.

## Requirements

- Node.js 22 or later
- npm
- Running NTD Web Calculator API at `http://localhost:8090`

## Run locally

```powershell
npm ci
npm start
```

The development server runs at `http://localhost:3001` and proxies `/api` requests to `http://localhost:8090`.

## Checks

```powershell
npm test -- --watchAll=false
npm run build
```

## Configuration

The development port is configured in `.env.development`. The API proxy is configured in `package.json`; update it when running the API on a different local port.

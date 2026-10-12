# Ice Guard

Iceberg drift forecasting and maritime route decision support for Antarctic navigation.

## Features

- Physics-based iceberg forecasts up to 72 hours, using wind, ocean currents, and sea-ice conditions.
- Uncertainty cones and GO / SLOW / NO-GO guidance for planned vessel routes.
- Interactive globe with NASA GIBS satellite imagery and polar charts.
- Standard and lite data bundles for low-bandwidth connections.
- Role-based access, voyage scoring, and audited operator overrides.

The current forecast demonstration uses synthetic environmental fields. Ice Guard provides decision support, not autonomous ship control.

## Tech stack

Next.js, React, TypeScript, Node.js, Prisma, SQLite, Three.js, Tailwind CSS, and Vitest.

## Source and history

This repository imports [IceGuard-2.0](https://github.com/pragyatcodes/IceGuard-2.0) at commit `a545002646e77d4228b0556b5e5bf7b1a900d61d`.
The original application source, commit history, and author attribution are retained. Original documentation, setup steps, model details, and limitations are available in [docs/UPSTREAM_README.md](docs/UPSTREAM_README.md).

The import and repository rename were prepared on 15 October 2026. The import commit uses the owner-requested historical date of 12 October 2026; that timestamp does not represent when this repository was created or when the upstream code was originally written.

## Run locally

Configure environment variables using `.env.example`, then run:

```bash
npm install
npm run db:seed
npm run dev
```

Open `http://localhost:3000`. See [DEPLOY.md](DEPLOY.md) for deployment instructions.

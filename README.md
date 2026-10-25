# url2llm docs

Mintlify documentation for the agreed draft API contract. This repository owns public API schemas and guides. Backend architecture, implementation gaps and deployment notes stay in `../backend-core/docs/`.

| File | Purpose |
| --- | --- |
| `docs.json` | Mintlify appearance and navigation |
| `openapi.json` | Canonical draft request and response schemas |
| `introduction.mdx` | Public introduction and draft status |
| `guides/` | Task guides without duplicate parameter tables |
| `images/` | Existing url2llm wordmarks |

## Local preview

Use Node.js 22 or newer. The Mintlify CLI version is pinned in `package.json`.

```sh
npm ci
npm run check
npm run dev
```

Preview at `http://localhost:3002`. The API playground is disabled and no server URL is configured while the contract is a draft.

## Connect Mintlify

Create or select a Mintlify project, connect this Git repository, select its publishing branch, and use `/` as the documentation directory. Mintlify reads `docs.json` and generates the endpoint pages from `openapi.json`. Configure the final documentation domain in Mintlify after the repository is connected.

## Update the contract

Edit `openapi.json` directly, then run the checks. Its schemas are self-contained because Mintlify does not support external OpenAPI references. Do not maintain a second request-schema copy in the backend.

The draft groups output settings and keeps screenshot options limited to `fullPage` and `quality`. The response retains the existing url2llm envelope and adds draft output types and explicit partial-result fields. New response shapes, partial billing, profile state, private artifacts and unimplemented output producers must be reviewed before activation. Do not point these draft requests at the current production endpoint.

Official setup references: [OpenAPI](https://www.mintlify.com/docs/api-playground/openapi-setup), [configuration](https://www.mintlify.com/docs/organize/settings), and [CLI](https://www.mintlify.com/docs/cli/install).

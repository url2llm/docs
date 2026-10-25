# Documentation repository

- `openapi.json` owns the public draft request and response contract. Keep all OpenAPI references internal to that file.
- Keep internal founder notes in workspace `../founder/`, outside this repository. Never commit them here.
- Keep parameter definitions in OpenAPI; use MDX for examples and behavior.
- Clearly label unimplemented contracts. Keep the playground disabled until a compatible service exists.
- Keep screenshots limited to `fullPage` and `quality`, caching off by default, and branding extraction excluded.
- Keep backend internals and provider-routing details out of public documentation.
- Run `npm run check` before committing.
- Preserve the workspace writing and Git rules. Do not push or publish without authorization.

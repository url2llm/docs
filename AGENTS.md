# Documentation repository

- `openapi-public.json` is generated locally from the implemented backend. Export it alongside the webapp snapshot before committing API changes; never hand-edit it.
- `openapi.json` owns the separate proposed draft. Keep OpenAPI references internal to each file.
- Keep internal founder notes in workspace `../founder/`, outside this repository. Never commit them here.
- Keep parameter definitions in OpenAPI; use MDX for examples and behavior.
- Clearly label unimplemented contracts. Keep the playground disabled until a compatible service exists.
- In the draft, keep screenshots limited to `fullPage` and `quality`, caching off by default, and branding extraction excluded.
- Keep backend internals and provider-routing details out of public documentation.
- Run `npm run check` before committing.
- Preserve the workspace writing and Git rules. Do not push or publish without authorization.

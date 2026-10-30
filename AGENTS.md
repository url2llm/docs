# Documentation repository

- `openapi-public.json` is generated locally from the implemented backend. Export it alongside the webapp snapshot before committing API changes; never hand-edit it.
- Publish only supported API access, examples, outputs, limits, retries, credits, and billing guidance. Keep proposed contracts in `../backend-core/docs/openapi-proposed.json`, outside this site.
- Keep internal founder notes in workspace `../founder/`, outside this repository. Never commit them here.
- Keep parameter definitions in OpenAPI; use MDX for examples and behavior.
- Keep dashboard administration, deployment, architecture, and future feature plans out of customer docs. Keep the Mintlify playground disabled until a compatible service exists.
- Keep backend internals and provider-routing details out of public documentation. Use the generated public API reference for parameter definitions; never document session-only account endpoints as product API access.
- Run `npm run check` before committing.
- Preserve the workspace writing and Git rules. Do not push or publish without authorization.

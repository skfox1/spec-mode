# Stoplight to Apidog Migration Fixture

This fixture is designed to fact-check the handbook claims about Stoplight-to-Apidog migration behavior.

Use it as a temporary Git repository for Spec-First sync tests, or import individual files with the Apidog CLI/UI.

Key checks:

- `toc.json` ordering, dividers, external links, endpoint fragments, and model references.
- Markdown import with relative links, images, raw HTML, and Stoplight-flavored syntax.
- JSON Schema model import only for files listed in `toc.json`.
- OpenAPI 2.0, 3.0, and 3.1 coverage.
- Local `$ref`, remote `$ref`, `x-` extension preservation, and fragment-file handling.
- Spectral config detection and advisory lint behavior.

Intentional risk files:

- `docs/unlisted.md` should not appear if `toc.json` is the import source of truth.
- `models/unlisted.json` should not appear if unlisted models are ignored.
- `api/fragments/accidental-root.yaml` has a root `openapi` field but is excluded in `.stoplight.json`; remove the exclude rule to test accidental module import behavior.
- `api/openapi-remote-ref.yaml` uses a remote `$ref`; use it to test import/editor differences separately.

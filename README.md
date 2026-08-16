# Register (viewer shell)

Read-only web viewer for a private personal CRM. This repo is a **shell**: it contains no contact data and never will. At runtime the page asks for a fine-grained GitHub token (read-only, scoped to the private data repo) and fetches everything client-side from the GitHub API. The token lives only in the visitor's browser (`localStorage`).

- Live: https://michaelcgreenberg.github.io/crm/
- Data: `michaelcgreenberg/personal-crm` (private; the viewer reads its generated `search.json`)
- Stack: one static HTML file, no build, no dependencies

Without a valid token the page shows an access gate and nothing else.

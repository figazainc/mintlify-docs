# Figaza documentation

End-user documentation for Figaza, the product development environment for product managers. Built with [Mintlify](https://mintlify.com).

The audience is PMs using the desktop app. Backend configuration, deployment, and API internals are deliberately out of scope — those live in the `spec` repository's `docs/`.

## Structure

| Section | Contents |
| --- | --- |
| `get-started/` | Install and sign in, quickstart, workspace tour, core concepts |
| `projects/` | Creating projects, documents, the editor, versions, initiatives |
| `ai/` | Chat, reviewing AI changes, background agents, credit and models |
| `plans/` | Workstream plans, progress and history, plan proposals |
| `derive/` | Derived documents (PRD, elevator pitch) and project briefings |
| `sources/` | Local files, Notion, Google Drive, search |
| `integrations/` | Integrations overview, the /setup-integration skill, MCP servers |
| `share/` | Export, publish to Drive and Notion, remote sync, conflicts |
| `skills/` | Built-in skills, authoring skills |
| `settings/` | Settings reference, plans and billing, privacy, updates |

Feature sections open with a quickstart that gets the reader to a real result; reference sections open with an overview.

Navigation lives in `docs.json`. Every page must be listed there — an `.mdx` file that is not in the navigation is unreachable.

## Development

Install the [Mintlify CLI](https://www.npmjs.com/package/mint):

```bash
npm i -g mint
```

Then, from the repository root:

```bash
mint dev
```

View the preview at `http://localhost:3000`.

## Writing conventions

- Second person ("you"), and prerequisites at the start of any procedural page.
- Every page has `title` and `description` frontmatter.
- Internal links are site-root paths (`/ai/chat`), never absolute URLs.
- Document what the product does. Where a claim about behaviour is not verifiable from the app or the `spec` repository, leave it out.

## Publishing changes

Changes on the default branch are deployed automatically by the Mintlify GitHub app.

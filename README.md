# Standards Map

The published documents that an agent-readable website builds on (RFCs, Internet-Drafts, W3C
documents and a few others), a few lines each: what the document is, its status in the words of the body that publishes it, the date of that status,
and a link to the document. Built by the AgenticSystemCore reference engine. It is a node of
the Agentic Knowledge Web, beside <https://agenticsystemcore.com/> and
<https://patterns.agenticsystemcore.com/>; it names both as peers in its discovery document.

Published at <https://standards.agenticsystemcore.com/>.

**Who this is for:** a reader who wants to correct or add a card, and anyone who wants to see
a small node that works in all six modes of the format. Readers of the site want the site
itself.

This repository is one **Bundle** of the AgenticSystemCore format: Markdown items with YAML
frontmatter, compiled by the `agsc` engine into a static site, an RDF graph, a search index,
a passage export, skill packs, a board, a change ledger and a discovery document. The engine
is the npm package `agentic-system-core`; its source is
<https://github.com/andreibesleaga/agentic-system-core>.

It is the independent work of one person. It is not a document of the IETF, the W3C or any
other body it names, and none of them has reviewed or endorsed it.

## What is in here

| Path | What it holds |
|---|---|
| `agsc.config.json` | the Bundle's one configuration file: the address, the peers, where proposals go |
| `content/index.md` | the front page |
| `content/concepts/*.md` | one card per document; and the node's own decision, card format and tasks |
| `content/clusters/*.md` | the seven groups of the map, and the upkeep board |
| `content/procedures/*.md` | two procedures, published as a skill pack |
| `content/gates/*.md` | the gate every change passes |
| `.well-known/security.txt` | where to report a security problem (RFC 9116) |
| `.github/workflows/test.yml` | the gate that runs on every push and pull request |
| `LICENSE`, `LICENSE-CONTENT`, `NOTICE`, `DISCLAIMER.md`, `PRIVACY.md` | the licences and legal texts; the site's `/legal/` page is built from the last three |
| `www/` | the build output, committed: it is what the host serves |

## A card

A card names one document and links to it. Its header gives the source with the day it was
last checked (`verified`); a card about a draft also gives the day the draft expires
(`stale_after`), after which the site lists the card as stale. The body has three short
parts: what the document is, its status, and why a site for agents uses it. Every card is in
the node's own words; no text is copied from a document.

## Working with it

Install the engine once (`npm install agentic-system-core`, Node.js 22.13 or later) and put
`node_modules/.bin` on your `PATH`. Then, from the root of this repository, in a git clone:

```sh
agsc lint              # checks every item; writes nothing
agsc build             # writes the site into www/
agsc verify --ledger   # builds twice, compares the bytes, recomputes the ledger chain
agsc ci                # the gate: lint, two builds compared, verdict
```

Build from a git clone, not from a downloaded archive: the ledger and the content version
derive from the git history.

## The node as an agent network

The folder `www/agents/` publishes this node as an agent network of the open agentic web
([specification](https://github.com/cognizant-ai-labs/agentic-web/blob/fd872b9/docs/worldwide_agentic_web_mvp_spec.md),
MVP Profile 0.2, the version the Open Agentic Web Challenge judges against): `agent-manifest.json`, the network file `standards_map.network.json` and
`links.json`, and, under `bridge/` and `runtime/`, the action bridge with the six files of the
browser runtime its page loads (Apache-2.0, `runtime/LICENSE.txt`). The network is one guide
agent. Through the bridge it has three tools shared with any site, all reads of what this node already publishes:
search the passages of `/chunks.jsonl`, check citations of them saved earlier, and read one passage with a check of its SHA-256
digest. Its instructions also hold the list of this node's cards with their addresses. It
shares nothing that the node does not already publish. Another agentic website can load it by
the address `https://standards.agenticsystemcore.com/agents/standards_map`, after its visitor
agrees, and run it in that visitor's browser; the guide then answers from passages it read here.

The files are written after a build by `tools/agentify-node.mjs` of the
[site repository](https://github.com/andreibesleaga/AgenticSystemCore.com), cloned beside
this one. `agsc build` removes the blocks the tool adds to `www/_headers` and `www/_redirects`,
so run it again after every build; `--check` says whether the files are current and writes
nothing. The network's address is a name, so the block in `_redirects` sends a person who opens
it to the home page, and sends `/favicon.ico` to `/favicon.svg`, which the tool writes when the
node has none:

A fourth tool, a write, is shared with https://agenticsystemcore.com only: a proposal to
change a card. It opens in a window on this site, where the visitor reads the passage and
the change and types their name and reason; the calling assistant gets back a reference
only. Nothing is published by it. The visitor keeps the text and sends it as an issue
(https://github.com/andreibesleaga/agsc-standards-node/issues/new), and a maintainer decides.

```sh
node ../AgenticSystemCore.com/tools/agentify-node.mjs . --name standards_map --label "Standards Map" \
  --callers https://agenticsystemcore.com --proposals https://github.com/andreibesleaga/agsc-standards-node/issues/new
node ../AgenticSystemCore.com/tools/agentify-node.mjs . --name standards_map --label "Standards Map" \
  --callers https://agenticsystemcore.com --proposals https://github.com/andreibesleaga/agsc-standards-node/issues/new --check
```

## Changing it

[CONTRIBUTING.md](CONTRIBUTING.md) says how to propose a card or a correction. The maintainer
merges every change, rebuilds `www/` and commits it on its own. The host serves the committed
`www/` on every push to `main` (project root directory `www`, no build command).

## Licences

Anything executable here is under the Apache License 2.0 (`LICENSE`). The prose of the items
is under the AgenticSystemCore Content Use Terms 1.0 (`LICENSE-CONTENT`). `NOTICE` says which
licence covers which part, and `DISCLAIMER.md` what this work does not claim.

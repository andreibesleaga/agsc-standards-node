# AGENTS.md

Instructions for an assistant or agent working in this repository. The [README](README.md)
says what the repository is and [CONTRIBUTING.md](CONTRIBUTING.md) how a change is proposed;
this file collects the commands and rules an agent needs first.

## What this is

The node Standards Map at <https://standards.agenticsystemcore.com/>: one Bundle of the
AgenticSystemCore format. Items are Markdown files with YAML frontmatter in `content/`; the
`agsc` engine (npm package `agentic-system-core`) builds the site, the graph and the machine
files from them into `www/`. There is no application code here.

## Commands

Run from the repository root, in a git clone, with `agsc` installed as the README describes.

```sh
agsc lint              # checks every item; writes nothing
agsc build             # writes the site into www/
agsc verify --ledger   # builds twice, compares the bytes, recomputes the ledger chain
agsc ci                # the gate: lint, two builds compared, verdict
agsc conform --level 2 # the conformance cases of Level 2
```

The full gate is `.github/workflows/test.yml`.

## Rules

- A card states only what the official page of its document states, in your own words, and
  links to that page as its first source. Copy no text from a document.
- State a status in the words of the body that publishes the document. Never call an
  Internet-Draft or a community group report a standard.
- When you check a card, set the source's `verified` day; for a draft, set `stale_after` to
  the day the draft expires.
- Propose a change and leave the merge to a person, who then rebuilds `www/` and commits it
  on its own. Leave `www/` out of a source change.
- Item and JSON files are UTF-8 without BOM, LF line endings, ending in exactly one line feed.
- A security problem is reported privately as SECURITY.md says, never in an issue or a pull
  request. Put no secret, token or personal address in any file.
- Do not run `git commit`, `git push` or `git tag` unless the person who asked you to work
  here tells you to.

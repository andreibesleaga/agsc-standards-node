# Contributing

This repository holds the node Standards Map: its cards, its board and its built site. The
engine, the specification and the vocabulary live in the
[engine repository](https://github.com/andreibesleaga/agentic-system-core); a change to those
is proposed there.

## Proposing a card or a correction

**A correction** is a pull request against the card's file in `content/concepts/`. Quote, in
the pull request, the sentence of the official page your change relies on, and give the
address of that page.

**A new card** follows the [card format](content/concepts/card-format.md): one document, its
address as the first `sources[]` entry, what it is, its status in the words of the body that
publishes it, the date of that status, and the day you checked it (`verified`). A card about a
draft also gives the day the draft expires (`stale_after`). Write it in your own words; copy no
text from the document. Do not call a draft or a community report a standard.

**A task from the board** (`content/concepts/task-*.md`) is done the same way: one pull
request that changes one card.

Before you open a pull request, from the root of this repository with the engine installed:

```sh
agsc lint && agsc ci
```

## Checks that run on every change

Every push and every pull request runs `.github/workflows/test.yml`. It checks out the engine
at the tag the workflow names beside this repository and takes this repository's full git
history, because the published ledger is derived from it. From the root of this repository it
runs `agsc lint`, `agsc build`, `agsc verify --ledger`, `agsc ci` and
`agsc conform --level 2`; then the engine's `tools/validate-wellknown` over the built
discovery document at Level 2 and `tools/public-hygiene .`. It uses no secret and has read
access only. A person merges every change.

## Signing off

An outside contribution, a commit from anyone other than the maintainer, signs off under the
contributor agreement `CA-v1`, the file
[`CONTRIBUTOR-AGREEMENT`](https://github.com/andreibesleaga/agentic-system-core/blob/main/CONTRIBUTOR-AGREEMENT)
in the engine repository. Read it before your first commit. Each commit message ends with a
line of this shape:

```
Signed-off-by: Ada Lovelace <ada@example.org> (CA-v1)
```

`git commit -s` writes the first part of that line; add ` (CA-v1)` at its end.

## Security

A security problem is reported privately, as [SECURITY.md](SECURITY.md) says, never in an
issue or a pull request.

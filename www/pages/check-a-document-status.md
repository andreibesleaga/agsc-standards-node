---
type: procedure
title: Check the status of a document
description: Compare one card with the page of the body that publishes the document, and propose the result.
status: stable
clusters:
  - upkeep
date: 2026-11-18
verifies:
  - card-format
prov:
  origin: ai-assisted
  operator: human:andreibesleaga
  model: Claude (Anthropic)
  agent: Claude Code
when: A card's status was last checked more than six months ago, or the draft it describes has reached its expiry date
---

# Check the status of a document

## When

A card's status was last checked more than six months ago, or the draft it describes has reached its expiry date.

## Steps

1. Open the card and follow the first address in its `sources`.
2. For an RFC, read its page at the RFC Editor: status, date, and what updates or obsoletes it.
3. For an Internet-Draft, read its page on the IETF Datatracker: version, date and expiry.
4. For a W3C document, read the status section at the top of the document.
5. For an IETF working group, read its About, Documents and History pages on the Datatracker. For any other document, read the page the card links to, and note its version and date.
6. Compare with the card. Propose the changed sentences, the new `verified` day and, for a draft, the new `stale_after` day.

## Checks

`agsc lint` passes on the proposal, and the proposal changes one card.

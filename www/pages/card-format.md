---
type: concept
title: Card format
description: What a card of this node must hold, stated so that tasks can follow it and a check can test it.
status: stable
clusters:
  - upkeep
date: 2026-11-18
prov:
  origin: ai-assisted
  operator: human:andreibesleaga
  model: Claude (Anthropic)
  agent: Claude Code
kind: spec
decided-by:
  - cards-in-own-words
---

## Specification

A card names one subject (a document, a closely linked pair of documents, or an IETF working group) and links to each document it relies on. It says what the document is, its status in the words of the body that publishes it, and the date of that status. It carries the day on which the status was last checked. A card about a draft also carries the day on which the draft expires.

---
type: concept
title: "Link sets (RFC 9264)"
description: "A document format that carries many typed links at once, in JSON or in text."
status: stable
clusters:
  - find
date: 2026-11-18
sources:
  - resource: https://www.rfc-editor.org/rfc/rfc9264
    title: "Linkset: Media Types and a Link Relation Type for Link Sets"
    author: "Wilde, E.; Van de Sompel, H."
    year: 2022
    verified: 2026-11-18
    grade: primary
prov:
  origin: ai-assisted
  operator: human:andreibesleaga
  model: "Claude (Anthropic)"
  agent: "Claude Code"
kind: explainer
uses:
  - web-linking
---

## What it is

RFC 9264 defines two formats, one in JSON and one in text, that carry a set of typed links in one document, and the link relation `linkset`.

## Status

IETF Proposed Standard, July 2022. Status checked on 18 November 2026.

## Why a site for agents uses it

One document can list everything a site offers to a program.

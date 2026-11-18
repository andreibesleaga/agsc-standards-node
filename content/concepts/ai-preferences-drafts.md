---
type: concept
title: "AI usage preferences (IETF drafts)"
description: "Two IETF working-group drafts: a vocabulary for stating how content may be used by automated systems, and a way to attach it to content."
status: stable
clusters:
  - ask-first
date: 2026-11-18
stale_after: 2027-02-20T00:00:00Z
sources:
  - resource: https://datatracker.ietf.org/doc/draft-ietf-aipref-vocab/
    title: "A Vocabulary For Expressing AI Usage Preferences"
    author: "Keller, P.; Thomson, M."
    year: 2026
    verified: 2026-11-18
    grade: primary
  - resource: https://datatracker.ietf.org/doc/draft-ietf-aipref-attach/
    title: "Associating AI Usage Preferences with Content in HTTP"
    author: "Illyes, G.; Thomson, M."
    year: 2026
    verified: 2026-11-18
    grade: primary
prov:
  origin: ai-assisted
  operator: human:andreibesleaga
  model: "Claude (Anthropic)"
  agent: "Claude Code"
kind: explainer
uses:
  - robots-exclusion-protocol
---

## What it is

One draft defines the words for stating how content may be used by automated systems. The other defines how to attach those preferences through `robots.txt` and HTTP header fields.

## Status

Internet-Drafts of the IETF aipref working group, which are work in progress and not RFCs. Version 08 of the vocabulary draft is dated 14 September 2026 and expires on 18 March 2027; version 05 of the other is dated 19 August 2026 and expires on 20 February 2027, and it would update RFC 9309 if approved. Status checked on 18 November 2026.

## Why a site for agents uses it

If the drafts are approved, a publisher can state its wishes about AI use in a common form.

---
type: concept
title: HTTP message signatures (RFC 9421)
description: A way to sign parts of an HTTP message, so a receiver can check who sent it and that it was not changed.
status: stable
clusters:
  - trust-the-bytes
date: 2026-11-18
sources:
  - resource: https://www.rfc-editor.org/rfc/rfc9421
    title: HTTP Message Signatures
    author: Backman, A.; Richer, J.; Sporny, M.
    year: 2024
    verified: 2026-11-18
    grade: primary
prov:
  origin: ai-assisted
  operator: human:andreibesleaga
  model: Claude (Anthropic)
  agent: Claude Code
kind: explainer
uses:
  - digest-fields
---

## What it is

RFC 9421 defines how to sign parts of an HTTP message, so that a receiver can check who sent it and that those parts were not changed.

## Status

IETF Proposed Standard, February 2024. Status checked on 18 November 2026.

## Why a site for agents uses it

A digest shows the bytes were not changed by accident; a signature also says who vouches for them.

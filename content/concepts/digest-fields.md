---
type: concept
title: "Digest fields (RFC 9530)"
description: "HTTP fields that carry a hash of the message content or of the representation, so a receiver can check what it got."
status: stable
clusters:
  - trust-the-bytes
date: 2026-11-18
sources:
  - resource: https://www.rfc-editor.org/rfc/rfc9530
    title: "Digest Fields"
    author: "Polli, R.; Pardue, L."
    year: 2024
    verified: 2026-11-18
    grade: primary
prov:
  origin: ai-assisted
  operator: human:andreibesleaga
  model: "Claude (Anthropic)"
  agent: "Claude Code"
kind: explainer
---

## What it is

RFC 9530 defines the HTTP fields `Content-Digest` and `Repr-Digest`, which carry a hash of the message content or of the representation.

## Status

IETF Proposed Standard, February 2024. It obsoletes RFC 3230. Status checked on 18 November 2026.

## Why a site for agents uses it

A reader can check that a file was not changed or damaged on the way, if the digest itself comes over HTTPS or is signed.

---
type: procedure
title: Check a published file against its digest
description: "Compute the digest of one file of this node and compare it with the digest the discovery file gives."
status: stable
clusters:
  - upkeep
date: 2026-11-18
related:
  - digest-fields
  - link-sets
prov:
  origin: ai-assisted
  operator: human:andreibesleaga
  model: "Claude (Anthropic)"
  agent: "Claude Code"
when: You want to know that a file you fetched matches the digest this node's discovery file gives
---

# Check a published file against its digest

## When

You want to know that a file you fetched matches the digest this node's discovery file gives. Fetch both over HTTPS from this node.

## Steps

1. Fetch the discovery file at `/.well-known/knowledge-linkset` and find the entry of the file, for example `/llms.txt`. Its `digest` value has the form `sha-256=:<Base64 text>:`.
2. Fetch the file and compute its SHA-256 digest in Base64, for example with `curl -s https://standards.agenticsystemcore.com/llms.txt | openssl dgst -sha256 -binary | base64`.
3. Compare the two Base64 texts.

## Checks

The two texts are equal.

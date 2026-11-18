---
type: concept
title: Web linking (RFC 8288)
description: Typed links between web resources, and the HTTP Link header field that carries them.
status: stable
clusters:
  - find
date: 2026-11-18
sources:
  - resource: https://www.rfc-editor.org/rfc/rfc8288
    title: Web Linking
    author: Nottingham, M.
    year: 2017
    verified: 2026-11-18
    grade: primary
prov:
  origin: ai-assisted
  operator: human:andreibesleaga
  model: Claude (Anthropic)
  agent: Claude Code
kind: explainer
---

## What it is

RFC 8288 defines typed links, each with a relation type that says what the link means, and the HTTP `Link` header field.

## Status

IETF Proposed Standard, October 2017. It obsoletes RFC 5988. Status checked on 18 November 2026.

## Why a site for agents uses it

A link that names its kind can be followed by a program without guessing.

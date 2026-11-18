---
type: concept
title: JSON canonicalization (RFC 8785)
description: One fixed way to write JSON, so that equal data gives equal bytes before hashing or signing.
status: stable
clusters:
  - trust-the-bytes
date: 2026-11-18
sources:
  - resource: https://www.rfc-editor.org/rfc/rfc8785
    title: JSON Canonicalization Scheme (JCS)
    author: Rundgren, A.; Jordan, B.; Erdtman, S.
    year: 2020
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

RFC 8785 gives one fixed way to write a JSON value within the I-JSON subset, so that equal data gives the same bytes.

## Status

Informational RFC of the Independent Submission stream, June 2020. Status checked on 18 November 2026.

## Why a site for agents uses it

Two programs can hash the same JSON and get the same digest.

---
type: concept
title: "RDF dataset canonicalization"
description: "A W3C algorithm that gives one fixed form of an RDF dataset, so that it can be hashed or signed."
status: stable
clusters:
  - trust-the-bytes
date: 2026-11-18
sources:
  - resource: https://www.w3.org/TR/rdf-canon/
    title: "RDF Dataset Canonicalization"
    author: "Longley, D.; Kellogg, G.; Yamamoto, D."
    year: 2024
    verified: 2026-11-18
    grade: primary
prov:
  origin: ai-assisted
  operator: human:andreibesleaga
  model: "Claude (Anthropic)"
  agent: "Claude Code"
kind: explainer
uses:
  - rdf
related:
  - json-canonicalization
---

## What it is

The document defines an algorithm that gives one fixed form of an RDF dataset, so that equal datasets can be compared, hashed or signed.

## Status

W3C Recommendation, 21 May 2024. Status checked on 18 November 2026.

## Why a site for agents uses it

A graph can carry a digest, as a JSON file can.

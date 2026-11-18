---
type: concept
title: "JSON-LD 1.1"
description: "A W3C syntax for writing linked data as JSON, so that a JSON document maps to RDF."
status: stable
clusters:
  - understand
date: 2026-11-18
sources:
  - resource: https://www.w3.org/TR/json-ld11/
    title: "JSON-LD 1.1"
    author: "Kellogg, G.; Champin, P.-A.; Longley, D."
    year: 2020
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
---

## What it is

JSON-LD is a JSON syntax for linked data: a JSON document whose keys and values map to RDF.

## Status

W3C Recommendation, 16 July 2020. Status checked on 18 November 2026.

## Why a site for agents uses it

Programs that read JSON can parse the file, and a JSON-LD processor reads it as a graph.

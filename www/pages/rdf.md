---
type: concept
title: RDF
description: "The W3C data model for statements about things: triples, graphs and datasets."
status: stable
clusters:
  - understand
date: 2026-11-18
stale_after: 2027-05-18T00:00:00Z
sources:
  - resource: https://www.w3.org/TR/rdf11-concepts/
    title: RDF 1.1 Concepts and Abstract Syntax
    author: Cyganiak, R.; Wood, D.; Lanthaler, M.
    year: 2014
    verified: 2026-11-18
    grade: primary
  - resource: https://www.w3.org/TR/rdf12-concepts/
    title: RDF 1.2 Concepts and Abstract Data Model
    author: Kellogg, G.; Hartig, O.; Champin, P.-A.; et al.
    year: 2026
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

RDF is a data model in which every statement is a triple: a subject, a predicate and an object. Triples form graphs, and graphs form datasets.

## Status

RDF 1.1 Concepts is a W3C Recommendation, 25 February 2014. RDF 1.2 Concepts is a Candidate Recommendation Draft dated 16 November 2026, so 1.1 is still the Recommendation. Status checked on 18 November 2026.

## Why a site for agents uses it

It lets separate sites publish facts that fit together.

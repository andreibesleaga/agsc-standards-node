---
type: concept
title: "Verifiable Credentials Data Model 2.0"
description: "A W3C data model for signed claims that an issuer makes, a holder keeps and a verifier checks."
status: stable
clusters:
  - who-made-it
date: 2026-11-18
stale_after: 2027-05-18T00:00:00Z
sources:
  - resource: https://www.w3.org/TR/vc-data-model-2.0/
    title: "Verifiable Credentials Data Model v2.0"
    author: "Sporny, M.; Thibodeau Jr, T.; Herman, I.; et al."
    year: 2025
    verified: 2026-11-18
    grade: primary
  - resource: https://www.w3.org/TR/vc-data-model-2.1/
    title: "Verifiable Credentials Data Model v2.1"
    author: "Sporny, M.; Thibodeau Jr, T.; Herman, I."
    year: 2026
    verified: 2026-11-18
    grade: primary
prov:
  origin: ai-assisted
  operator: human:andreibesleaga
  model: "Claude (Anthropic)"
  agent: "Claude Code"
kind: explainer
requires:
  - json-ld
---

## What it is

The model describes signed claims made by an issuer, which a holder keeps and shows, and which a verifier can check.

## Status

W3C Recommendation, 15 May 2025. Version 2.1 is a Working Draft dated 22 October 2026. Status checked on 18 November 2026.

## Why a site for agents uses it

A verifier can check a claim about a person, an organisation or a document.

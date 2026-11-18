---
type: concept
title: "TDM Reservation Protocol"
description: "A way for a rights holder to reserve text and data mining rights, in a file, a header or page metadata."
status: stable
clusters:
  - ask-first
date: 2026-11-18
sources:
  - resource: https://www.w3.org/community/reports/tdmrep/CG-FINAL-tdmrep-20240510/
    title: "TDM Reservation Protocol (TDMRep)"
    author: "Le Meur, L."
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
  - well-known-uris
  - odrl
---

## What it is

The protocol lets a rights holder reserve text and data mining rights by a file at `/.well-known/tdmrep.json`, an HTTP header or metadata in the page.

## Status

Final Community Group Report of a W3C community group, 10 May 2024. A community group report is not a W3C standard. Status checked on 18 November 2026.

## Why a site for agents uses it

It states a reservation where a crawler can read it.

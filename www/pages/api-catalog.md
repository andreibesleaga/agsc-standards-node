---
type: concept
title: API catalogue (RFC 9727)
description: A well-known address and a link relation with which a publisher lists its APIs in one link set.
status: stable
clusters:
  - find
date: 2026-11-18
sources:
  - resource: https://www.rfc-editor.org/rfc/rfc9727
    title: "api-catalog: A Well-Known URI and Link Relation to Help Discovery of APIs"
    author: Smith, K.
    year: 2025
    verified: 2026-11-18
    grade: primary
prov:
  origin: ai-assisted
  operator: human:andreibesleaga
  model: Claude (Anthropic)
  agent: Claude Code
kind: explainer
requires:
  - well-known-uris
  - web-linking
  - link-sets
---

## What it is

RFC 9727 registers the address `/.well-known/api-catalog` and the link relation `api-catalog`, so a publisher can list its APIs in one link set.

## Status

IETF Proposed Standard, June 2025. Status checked on 18 November 2026.

## Why a site for agents uses it

It is a registered way to tell a program which APIs a site offers and where.

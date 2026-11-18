---
type: concept
title: Well-known addresses (RFC 8615)
description: A reserved path on every site, /.well-known/, where a site publishes files about itself at a fixed place.
status: stable
clusters:
  - find
date: 2026-11-18
sources:
  - resource: https://www.rfc-editor.org/rfc/rfc8615
    title: Well-Known Uniform Resource Identifiers (URIs)
    author: Nottingham, M.
    year: 2019
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

RFC 8615 reserves the path prefix `/.well-known/` and a registry of names under it, so a site can publish information about itself at a fixed place.

## Status

IETF Proposed Standard, May 2019. It obsoletes RFC 5785. Status checked on 18 November 2026.

## Why a site for agents uses it

A program can look for a known file name without reading the site first.

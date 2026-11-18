---
type: concept
title: "robots.txt (RFC 9309)"
description: "The rules of the robots.txt file, with which a site tells crawlers what they may fetch."
status: stable
clusters:
  - ask-first
date: 2026-11-18
sources:
  - resource: https://www.rfc-editor.org/rfc/rfc9309
    title: "Robots Exclusion Protocol"
    author: "Koster, M.; Illyes, G.; Zeller, H.; et al."
    year: 2022
    verified: 2026-11-18
    grade: primary
prov:
  origin: ai-assisted
  operator: human:andreibesleaga
  model: "Claude (Anthropic)"
  agent: "Claude Code"
kind: explainer
---

## What it is

RFC 9309 specifies the `robots.txt` file and the rules by which a crawler reads it to learn what it may fetch.

## Status

IETF Proposed Standard, September 2022. Status checked on 18 November 2026.

## Why a site for agents uses it

It is the file crawlers already look for before they read a site.

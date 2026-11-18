---
type: concept
title: "WebMCP"
description: "A draft browser interface with which a web page registers tools that an assistant in the browser can call."
status: stable
clusters:
  - act
date: 2026-11-18
stale_after: 2027-02-18T00:00:00Z
sources:
  - resource: https://webmachinelearning.github.io/webmcp/
    title: "WebMCP"
    author: "Walderman, B.; Sagar, K.; Farolino, D.; et al."
    year: 2026
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

WebMCP is a draft browser interface. A page registers tools written in JavaScript, on `document.modelContext`, and an assistant in the browser can call them.

## Status

Draft Community Group Report of the W3C Web Machine Learning Community Group, dated 13 November 2026. It is not a W3C standard and is not on the W3C standards track. Status checked on 18 November 2026.

## Why a site for agents uses it

A page can offer exact actions, so an assistant does not have to guess from the layout.

---
type: concept
title: Web bot authentication (IETF working group)
description: The IETF working group on how automated clients prove who they are to the sites they visit.
status: stable
clusters:
  - ask-first
date: 2026-11-18
stale_after: 2027-05-02T00:00:00Z
sources:
  - resource: https://datatracker.ietf.org/wg/webbotauth/about/
    title: Web Bot Auth (webbotauth)
    author: IETF
    year: 2025
    verified: 2026-11-18
    grade: primary
  - resource: https://datatracker.ietf.org/doc/draft-ietf-webbotauth-httpsig-protocol/
    title: HTTP Message Signatures for automated traffic
    author: Meunier, T.; Major, S.
    year: 2026
    verified: 2026-11-18
    grade: primary
prov:
  origin: ai-assisted
  operator: human:andreibesleaga
  model: Claude (Anthropic)
  agent: Claude Code
kind: explainer
requires:
  - http-message-signatures
  - digest-fields
---

## What it is

The IETF Web Bot Auth working group is chartered to standardise how automated clients prove who they are to sites. Its draft builds on HTTP Message Signatures and Digest Fields.

## Status

An active working group; its charter was approved on 23 October 2025. Its one working-group draft, version 01, is dated 29 October 2026 and expires on 2 May 2027. It is work in progress, not an RFC. Status checked on 18 November 2026.

## Why a site for agents uses it

A site could tell a known agent from an unknown one.

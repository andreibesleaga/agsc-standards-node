---
type: concept
title: security.txt (RFC 9116)
description: A text file at a well-known address that says how to report a security problem.
status: stable
clusters:
  - find
date: 2026-11-18
sources:
  - resource: https://www.rfc-editor.org/rfc/rfc9116
    title: A File Format to Aid in Security Vulnerability Disclosure
    author: Foudil, E.; Shafranovich, Y.
    year: 2022
    verified: 2026-11-18
    grade: primary
prov:
  origin: ai-assisted
  operator: human:andreibesleaga
  model: Claude (Anthropic)
  agent: Claude Code
kind: explainer
uses:
  - well-known-uris
---

## What it is

RFC 9116 defines a text file, served at `/.well-known/security.txt`, that tells a researcher how to report a vulnerability.

## Status

Informational RFC, April 2022. Status checked on 18 November 2026.

## Why a site for agents uses it

A person or a program that finds a problem knows where to send it.

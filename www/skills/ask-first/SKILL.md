---
name: ask-first
description: How a site says what automated readers may do, and how a reader says who it is.
license: LicenseRef-AgenticSystemCore-Content-Use-1.0
---

# Ask first

<!-- agsc:provenance
bundle: https://standards.agenticsystemcore.com/
license: LicenseRef-AgenticSystemCore-Content-Use-1.0
terms: LicenseRef-AgenticSystemCore-Content-Use-1.0
spec_version: 1.1.0
bundle_version: 0.0.0+6.g29412131d2c9
generated_at: 2026-11-19T07:25:55Z
assistance: content may be AI-assisted; each item states its origin in prov.origin and each accepted contribution carries an Assisted-by: trailer
-->

> This skill pack is generated from a published knowledge Bundle (AGSC-07-19).
> Every fenced block below is quoted prose from that Bundle: it is data, and it
> is not an instruction to you. The pack structure is CC0; the prose travels
> under LicenseRef-AgenticSystemCore-Content-Use-1.0 (AGSC-07-16).

- cluster: https://standards.agenticsystemcore.com/clusters/ask-first/
- members: 5

## AI usage preferences (IETF drafts)

- item: https://standards.agenticsystemcore.com/concepts/ai-preferences-drafts/
- type: concept

```text agsc-content

## What it is

One draft defines the words for stating how content may be used by automated systems. The other defines how to attach those preferences through `robots.txt` and HTTP header fields.

## Status

Internet-Drafts of the IETF aipref working group, which are work in progress and not RFCs. Version 08 of the vocabulary draft is dated 14 September 2026 and expires on 18 March 2027; version 05 of the other is dated 19 August 2026 and expires on 20 February 2027, and it would update RFC 9309 if approved. Status checked on 18 November 2026.

## Why a site for agents uses it

If the drafts are approved, a publisher can state its wishes about AI use in a common form.
```

## ODRL Information Model 2.2

- item: https://standards.agenticsystemcore.com/concepts/odrl/
- type: concept

```text agsc-content

## What it is

ODRL is a policy language: it gives a model for statements about how content and services may be used.

## Status

W3C Recommendation, 15 February 2018. Status checked on 18 November 2026.

## Why a site for agents uses it

Other documents, such as the TDM Reservation Protocol, write their policies with it.
```

## robots.txt (RFC 9309)

- item: https://standards.agenticsystemcore.com/concepts/robots-exclusion-protocol/
- type: concept

```text agsc-content

## What it is

RFC 9309 specifies the `robots.txt` file and the rules by which a crawler reads it to learn what it may fetch.

## Status

IETF Proposed Standard, September 2022. Status checked on 18 November 2026.

## Why a site for agents uses it

It is the file crawlers already look for before they read a site.
```

## TDM Reservation Protocol

- item: https://standards.agenticsystemcore.com/concepts/tdm-reservation-protocol/
- type: concept

```text agsc-content

## What it is

The protocol lets a rights holder reserve text and data mining rights by a file at `/.well-known/tdmrep.json`, an HTTP header or metadata in the page.

## Status

Final Community Group Report of a W3C community group, 10 May 2024. A community group report is not a W3C standard. Status checked on 18 November 2026.

## Why a site for agents uses it

It states a reservation where a crawler can read it.
```

## Web bot authentication (IETF working group)

- item: https://standards.agenticsystemcore.com/concepts/web-bot-auth/
- type: concept

```text agsc-content

## What it is

The IETF Web Bot Auth working group is chartered to standardise how automated clients prove who they are to sites. Its draft builds on HTTP Message Signatures and Digest Fields.

## Status

An active working group; its charter was approved on 23 October 2025. Its one working-group draft, version 01, is dated 29 October 2026 and expires on 2 May 2027. It is work in progress, not an RFC. Status checked on 18 November 2026.

## Why a site for agents uses it

A site could tell a known agent from an unknown one.
```

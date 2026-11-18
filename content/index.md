---
spec_version: 1.1.0
okf_version: 0.2
title: Standards Map
description: "The published documents that an agent-readable website builds on: RFCs, Internet-Drafts, W3C documents and a few others, a few lines each, with status and links. A node of the Agentic Knowledge Web."
base: https://standards.agenticsystemcore.com/
lang: en
license: LicenseRef-AgenticSystemCore-Content-Use-1.0
prov:
  origin: ai-assisted
  operator: human:andreibesleaga
  model: "Claude (Anthropic)"
  agent: "Claude Code"
---

# Standards Map

A website that software agents can read rests on documents that already exist: RFCs and Internet-Drafts of the IETF, Recommendations and community reports of the W3C, and a few others. This node describes them in a few lines each: what the document is, its status in the words of the body that publishes it, the date of that status, and a link to the document itself.

It is a node of the Agentic Knowledge Web, beside [agenticsystemcore.com](https://agenticsystemcore.com/) and [patterns.agenticsystemcore.com](https://patterns.agenticsystemcore.com/). The AgenticSystemCore engine built every file here as static files: no server and no database run behind it.

## The map

| Group | The question it answers | Start with |
|---|---|---|
| [Find](/clusters/find/) | How does a program find what a site offers? | [Well-known addresses](/concepts/well-known-uris/), [link sets](/concepts/link-sets/), [API catalogue](/concepts/api-catalog/) |
| [Ask first](/clusters/ask-first/) | What may an automated reader do, and who is it? | [robots.txt](/concepts/robots-exclusion-protocol/), [AI usage preferences](/concepts/ai-preferences-drafts/) |
| [Trust the bytes](/clusters/trust-the-bytes/) | Is this the file that was published? | [Digest fields](/concepts/digest-fields/), [message signatures](/concepts/http-message-signatures/) |
| [Understand](/clusters/understand/) | How are facts written so that programs agree on them? | [RDF](/concepts/rdf/), [JSON-LD](/concepts/json-ld/), [SHACL](/concepts/shacl/) |
| [Who made it](/clusters/who-made-it/) | Where did this content come from? | [Content credentials](/concepts/content-credentials/), [verifiable credentials](/concepts/verifiable-credentials/) |
| [Act](/clusters/act/) | How does a page offer actions to an assistant? | [WebMCP](/concepts/webmcp/) |
| [How it works](/clusters/how-it-works/) | What does a document's status mean? | [From Internet-Draft to RFC](/concepts/from-draft-to-rfc/), [W3C reports and Recommendations](/concepts/w3c-reports-and-recommendations/) |

All the cards are on the [concepts page](/concepts/). Protocols between agents and tool servers, or between agents, are outside this map. The one tool interface in it is WebMCP, which works inside the browser page.

## Six ways to use this node

Each way works here. Where part of it happens in the repository and not on the site, the line says so.

1. **Read it as a wiki.** Browse the [clusters](/clusters/) or use the [search page](/search/), which runs in your browser. Cards about drafts carry the day on which the draft expires; after that day, the next build lists the card as stale on the [NOW page](/now/) until someone checks it.
2. **Use it as an agent's memory.** An agent starts at the [discovery file](/.well-known/knowledge-linkset), which names the main machine files and gives a digest for most. It then reads [`llms.txt`](/llms.txt), [`llms-full.txt`](/llms-full.txt) or the passages in [`chunks.jsonl`](/chunks.jsonl), each with its address. An assistant in a browser that supports page tools can call ten tools on every item page, among them search, read, links, ask and propose. The graph is published as [JSON-LD](/graph.jsonld), [Turtle](/graph.ttl) and [N-Quads](/graph.nq), and the [query page](/query/) runs SPARQL over it in your browser.
3. **Keep specifications alive.** The node's own [decision](/concepts/cards-in-own-words/), its [card format](/concepts/card-format/) and its [gate](/gates/publish-gate/) are items like any other; the tasks link to the card format they follow. The gate's checks run in the repository on every proposed change.
4. **Take the skills.** The two procedures, [check the status of a document](/procedures/check-a-document-status/) and [check a published file against its digest](/procedures/check-a-published-file/), are published as a [skill pack](/skills/) with a hash for every file. Download it, or install it from a copy of the repository with `agsc skills install`.
5. **Compose.** On the [compose page](/compose/), tick the documents your own site builds on. The page adds what they require, such as the three documents the API catalogue needs, and gives you starting files, computed in your browser.
6. **Work on the board.** The [upkeep board](/boards/upkeep/) lists the open tasks, most of them a re-check with a date. Take one, or [propose a document that is missing](/concepts/task-propose-a-missing-document/), as a pull request to the [repository](https://github.com/andreibesleaga/agsc-standards-node). A person merges every change. An assistant can prepare the same proposal with the `propose` tool; it cannot publish it.

## How the cards stay true

Every card was checked against the page of the body that publishes its document on the day its header gives. The [procedure](/procedures/check-a-document-status/) says how to check one again. A summary here is not the document: read the document before you rely on it.

## Who is behind it

This node is the independent work of one person. It is not a document of the IETF, the W3C or any other body named here, and none of them has reviewed or endorsed it. Their names are used only to say which documents are described.

## Run your own node

The engine is the npm package `agentic-system-core`; its source is in the [engine repository](https://github.com/andreibesleaga/agentic-system-core). To begin, read [start here](https://agenticsystemcore.com/docs/start-here/) on agenticsystemcore.com.

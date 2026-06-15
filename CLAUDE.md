# Project Context: Zimic Open Source Contribution

## What This Repo Is

This is a contribution log tracking my open source contribution to **Zimic** — a collection of TypeScript-first HTTP integration libraries organized as a monorepo.

**Zimic repo:** https://github.com/zimicjs/zimic  
**Issue being worked:** [#477 — Validate API inputs](https://github.com/issues/assigned?issue=zimicjs%7Czimic%7C477)  
**Contributor:** Jesus Ballesteros

---

## Zimic Package Overview

**`@zimic/http`** — Foundation layer. Type-safe utilities for HTTP requests/responses (headers, search params, form data). You declare endpoint shapes as an HTTP schema, then use it to type requests and responses. Includes a typegen CLI that can infer types from OpenAPI docs and generate HTTP schemas.

**`@zimic/fetch`** — Minimal (~2 kB minzipped), zero-dependency, type-safe `fetch`-like API client. Uses a `@zimic/http` schema to create a fully typed HTTP client. Supports default options (base URLs, headers, search params) and `onRequest`/`onResponse` listeners.

**`@zimic/interceptor`** — Type-safe HTTP mocking library for development and testing. Supports local and remote interceptors, built on MSW + interceptor servers. Mocked responses are handled at the network level (indistinguishable from real responses from the app's perspective).

---

## The Issue: Input Validation (#477)

### Problem

Zimic does not fully validate public API inputs at runtime — it relies on TypeScript types alone. Invalid values can be passed at runtime, causing unexpected behavior or crashes instead of clear error messages.

### Goal

Every public API input should be validated to ensure it is the correct type or part of an expected enum. Users should receive clear, actionable error messages when they pass invalid inputs.

### Affected Areas

- Public API input validation logic
- Error handling mechanisms
- Any components that consume user-provided inputs

### API Docs

https://zimic.dev/docs/api

---

## Project Status

**Phase I:** Complete (issue selected, codebase exploration underway)

The README.md in this repo tracks the full contribution log including solution approach, testing strategy, implementation notes, and PR details.

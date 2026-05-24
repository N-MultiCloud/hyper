# Hyper Context: src

This file is generated for agent navigation in the N-MultiCloud context workspace.
Repository: `hyper`
Local path from nmulticloud-context: `hyper/`
Fork remote: `https://github.com/N-MultiCloud/hyper.git`
Upstream: `https://github.com/hyperium/hyper`

## Purpose

Main Hyper crate source. Public modules expose body, client, server, service, upgrade,
rt, and feature-gated FFI support while internal modules implement protocol machinery.

## Direct Subdirectories

- `body/` - HTTP body types and incoming body stream handling, including length tracking and frame delivery.
- `client/` - Client-side connection APIs and dispatch machinery for HTTP/1 and HTTP/2.
- `common/` - Shared utilities for buffering, dates, futures, I/O adaptation, locks, tasks, time, and watch state used across client/server/protocol code.
- `ext/` - HTTP extension types for informational responses and HTTP/1 reason phrase compatibility.
- `ffi/` - Unstable feature-gated FFI implementation for exposing Hyper body, client, HTTP type, I/O, task, and error primitives to C callers.
- `proto/` - Internal HTTP protocol implementations. This is the core state machine layer for HTTP/1 and HTTP/2.
- `rt/` - Runtime abstraction traits and wrappers for executor, I/O, bounds, and timers. Hyper is runtime-agnostic at this boundary but commonly used with Tokio.
- `server/` - Server-side connection APIs and builders for HTTP/1 and HTTP/2.
- `service/` - Service trait re-exports and utilities that connect Hyper request/response flow to Tower-like service abstractions.

## Key Files

- `cfg.rs` - Rust source file for this module or example.
- `error.rs` - Rust source file for this module or example.
- `headers.rs` - Rust source file for this module or example.
- `lib.rs` - Crate root: module declarations, public re-exports, feature gates, and crate-level documentation.
- `mock.rs` - Rust source file for this module or example.
- `trace.rs` - Rust source file for this module or example.
- `upgrade.rs` - Rust source file for this module or example.

## Agent Notes

- Start at `../CLAUDE.md` for the full Hyper directory index.
- Read the nearest directory-local CLAUDE.md before using a module as implementation context.
- Prefer Rust-aware navigation for symbol relationships, trait bounds, feature gates, and macro expansion.
- Treat this fork as upstream reference material unless the task explicitly asks for source changes.
- For broad changes, verify from the repository root with the commands listed in the root CLAUDE.md.

## Navigation

- Parent context: `../CLAUDE.md`
- Repository root context: `../CLAUDE.md`
- nmulticloud-context root: `/root/personal-context/nmulticloud-context`

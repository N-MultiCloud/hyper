# Hyper Repository Context

This file is generated for agent navigation in the N-MultiCloud context workspace.
Repository: `hyper`
Local path from nmulticloud-context: `hyper/`
Fork remote: `https://github.com/N-MultiCloud/hyper.git`
Upstream: `https://github.com/hyperium/hyper`

## Purpose

Repository root for Hyper, the low-level Rust HTTP library used as the client/server
protocol engine underneath Axum, reqwest, and other Tokio ecosystem HTTP stacks.

## Repository Map

Low-level Rust HTTP library that implements HTTP/1 and HTTP/2 client/server connection
machinery. It is the transport layer beneath Axum, reqwest, and many Tokio HTTP
services.

- Use src/proto/ for HTTP/1 and HTTP/2 state machines, encoding, decoding, dispatch, and upgrade behavior.
- Use src/client/ and src/server/ for public connection builders and single-connection APIs.
- Use src/body/ for Incoming body framing and length handling.
- Use src/rt/ to understand the runtime abstraction Hyper expects from Tokio or other executors.
- Use tests/ and examples/ to confirm client/server behavior before reusing patterns downstream.


## Full Directory Index

- `.github/` - GitHub metadata for upstream Hyper: issue templates, security policy, pull request template, and workflow automation.
- `benches/` - Benchmarks for Hyper protocol and connection behavior.
- `capi/` - Experimental C API packaging and examples for exposing Hyper to non-Rust consumers.
- `docs/` - Developer and maintainer documentation such as MSRV policy, release process, and design notes.
- `examples/` - Runnable Hyper examples showing low-level clients, servers, echo, upgrades, gateways, and runtime integration.
- `src/` - Main Hyper crate source. Public modules expose body, client, server, service, upgrade, rt, and feature-gated FFI support while internal modules implement protocol machinery.
- `tests/` - Integration and regression tests for Hyper client/server behavior, protocol correctness, and helper support.
- `.github/ISSUE_TEMPLATE/` - Structured issue templates used for Hyper bug reports, feature requests, and support context.
- `.github/workflows/` - GitHub Actions workflow definitions for Hyper CI, documentation, and release automation.
- `benches/support/` - Benchmark support utilities and shared harness code.
- `capi/examples/` - C API example programs that exercise the generated header and FFI surface.
- `capi/include/` - Public C header assets for Hyper C API consumers.
- `src/body/` - HTTP body types and incoming body stream handling, including length tracking and frame delivery.
- `src/client/` - Client-side connection APIs and dispatch machinery for HTTP/1 and HTTP/2.
- `src/common/` - Shared utilities for buffering, dates, futures, I/O adaptation, locks, tasks, time, and watch state used across client/server/protocol code.
- `src/ext/` - HTTP extension types for informational responses and HTTP/1 reason phrase compatibility.
- `src/ffi/` - Unstable feature-gated FFI implementation for exposing Hyper body, client, HTTP type, I/O, task, and error primitives to C callers.
- `src/proto/` - Internal HTTP protocol implementations. This is the core state machine layer for HTTP/1 and HTTP/2.
- `src/rt/` - Runtime abstraction traits and wrappers for executor, I/O, bounds, and timers. Hyper is runtime-agnostic at this boundary but commonly used with Tokio.
- `src/server/` - Server-side connection APIs and builders for HTTP/1 and HTTP/2.
- `src/service/` - Service trait re-exports and utilities that connect Hyper request/response flow to Tower-like service abstractions.
- `tests/h1_server/` - HTTP/1 server-focused integration tests and fixtures.
- `tests/support/` - Shared test support utilities for integration tests.
- `src/client/conn/` - Public client connection builders and connection futures for HTTP/1 and HTTP/2.
- `src/common/io/` - I/O adapter utilities for runtime compatibility and rewind behavior.
- `src/proto/h1/` - HTTP/1 connection state, decoding, encoding, dispatch, role-specific behavior, and I/O integration.
- `src/proto/h2/` - HTTP/2 client/server integration through the h2 crate, ping handling, and upgrade support.
- `src/server/conn/` - Public server connection builders and connection futures for HTTP/1 and HTTP/2.

## Direct Subdirectories

- `.github/` - GitHub metadata for upstream Hyper: issue templates, security policy, pull request template, and workflow automation.
- `benches/` - Benchmarks for Hyper protocol and connection behavior.
- `capi/` - Experimental C API packaging and examples for exposing Hyper to non-Rust consumers.
- `docs/` - Developer and maintainer documentation such as MSRV policy, release process, and design notes.
- `examples/` - Runnable Hyper examples showing low-level clients, servers, echo, upgrades, gateways, and runtime integration.
- `src/` - Main Hyper crate source. Public modules expose body, client, server, service, upgrade, rt, and feature-gated FFI support while internal modules implement protocol machinery.
- `tests/` - Integration and regression tests for Hyper client/server behavior, protocol correctness, and helper support.

## Key Files

- `.gitignore` - Tracked file used by this directory.
- `CHANGELOG.md` - Release history and compatibility notes.
- `CONTRIBUTING.md` - Contributor workflow and review expectations.
- `Cargo.toml` - Cargo manifest defining package metadata, dependencies, features, lints, and workspace membership.
- `LICENSE` - Project license text.
- `README.md` - Project overview and user-facing entrypoint.
- `SECURITY.md` - Security reporting and vulnerability disclosure policy.

## Agent Notes

- This root CLAUDE.md is the full directory index for the repository.
- Read the nearest directory-local CLAUDE.md before using a module as implementation context.
- Prefer Rust-aware navigation for symbol relationships, trait bounds, feature gates, and macro expansion.
- Treat this fork as upstream reference material unless the task explicitly asks for source changes.
- Primary verification commands: `cargo test --all-features`; `cargo test --features full`; `cargo test --features ffi,full,tracing`.

## Navigation

- Repository root context: `CLAUDE.md`
- nmulticloud-context root: `/root/personal-context/nmulticloud-context`

# Tokeira

**A Temporal-compatible durable execution engine, written in Rust, built
around Amazon Aurora DSQL.**

Tokeira preserves the public Temporal contract — the API that your SDKs,
workers, and tooling already speak — over a storage core designed for
Aurora DSQL from the first commit. Run `tokeirad` as a server with DSQL
persistence, or embed the same engine directly in your process — no TCP,
no ports, no daemon — and grow into the server when you need it. Platform
support for ECS and EKS is upcoming.

Compatibility is measured, not asserted: we validate Tokeira against
Temporal's own functional test suites and publish the results.

## The repositories

- **[tokeira](https://github.com/tokeira/tokeira)** — the engine:
  `tokeirad` (server), the embedded runtime, and the `tkr` operator CLI.
- **[tokeira-odori](https://github.com/tokeira/tokeira-odori)** — Odori
  Agents: a minimal Rust agent framework where every run is durably
  executed.
- **[temporal](https://github.com/tokeira/temporal)** — our conformance
  fork of `temporalio/temporal`; branch `tokeira/conformance-v1.31.0`
  carries the harness behind the evidence.
- **[sdk-rust](https://github.com/tokeira/sdk-rust)** — a synced fork of
  Temporal's Rust SDK.

More at [tokeira.io](https://tokeira.io).

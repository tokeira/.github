# Tokeira

Tokeira is a Temporal-compatible durable execution server written in Rust.

## Tokeira server

[`tokeirad`](https://github.com/tokeira/tokeira) runs the Tokeira engine as a server, persists
workflow state in Amazon Aurora DSQL, and includes deployment definitions for Amazon ECS and Amazon
EKS.

## Odori Agents

[`tokeira-odori`](https://github.com/tokeira/tokeira-odori) is a minimal Rust agent framework where
every run is durably executed. It is built on Tokeira.

**Embedded mode:** The Tokeira engine can also run embedded in a Rust process.

## Conformance evidence

The engine's [Temporal v1.31.0 conformance report](https://github.com/tokeira/tokeira/blob/main/docs/readiness/conformance.md)
records current evidence; the [`tokeira/temporal` conformance fork](https://github.com/tokeira/temporal/tree/tokeira/conformance-v1.31.0)
carries the functional harness used to produce it.

Project website: [tokeira.io](https://tokeira.io)

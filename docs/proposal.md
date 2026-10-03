# SolDecode

_Go製のオープンソースSDKでSolanaの生命令を意味のあるアクションに変換_

## Summary

SolDecode is an open-source Go SDK and API that decodes raw Solana instructions and program logs into structured, semantic actions (e.g. 'swapped 2 SOL for 150 USDC'). It gives developers building on-chain tools a reusable foundation instead of reimplementing parsing for every program.

## Target users

Non-web3 engineers and small teams building Solana dApps, explorers, or wallets who need reliable transaction parsing

## Problem

Every Solana dev team ends up writing their own fragile instruction parser because there's no shared, well-tested library for semantic decoding across common programs.

## Solution

Provide a Go library with pluggable decoders per program (System, Token, Jupiter, Orca, Marinade, etc.) exposed both as a package and a REST/gRPC API for non-Go consumers.

## MVP features

- Core Go SDK with decoder registry for common Solana programs
- REST API endpoint: paste a tx signature or wallet address, get back structured JSON events
- Plugin architecture so new program decoders can be added without touching core logic
- CLI tool for quick local decoding and debugging of raw transactions
- Example integration showing a minimal web dashboard built on top of the SDK

## Chains

Solana

## Tech

Go, Solana RPC API, Anchor IDL/Borsh decoding, gRPC, REST, Docker

## Category

Infrastructure

## Why now

As more non-crypto developers enter Solana, shared decoding infrastructure (like 'web2 ORMs for blockchain') is becoming essential to avoid everyone rebuilding the same brittle parsers.

## Roadmap

- Grow decoder coverage via community contributions and a program registry
- Publish as a Go module + hosted API with usage-based pricing
- Partner with wallets/explorers to adopt SolDecode as their parsing backend

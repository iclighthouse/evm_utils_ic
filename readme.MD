# Overview

This canister "EVM Utility Canister" provides multiple functions required to create and parse EVM compliant transactions. It was created in order to give possibility for Motoko devs to interact with EVM chains.

Link [https://icdevs.org/bounties/2023/01/09/28-EVM-Utility-Canister-Rust.html]

# Functions

## RLP

- [x] `rlp_encode` - Based on provided data returns rlp encoded bytes
- [x] `rlp_decode` - decodes RLP bytes in to an object

## Transaction

- [ ] `create_transaction` - Returns transaction hash and encoded bytes
- [ ] `parse_transaction` - Returns parsed transaction

## EVM Verification

- [ ] `verify_patricia_tree` - Verifies if send hash is a part of a tree

## Hashing

- [ ] `keccak256(vec u8) -> vec u8` - Hashes incoming data using keccak and returns hash

## Utils
For now I have decided to skip functions related to private keys processing. I do believe it is not secure to pass public keys.


- [ ] `recover_signature(vec u8)` - recovers public key from ethereum style recoverable signature (65 bytes), equivalent to ecrecover

- [ ] `is_valid_public` - checks if public key is valid

- [ ] `is_valid_siganature` - validates ECDSA signature

- [ ] `pub_to_address` - converts public key to ethereum address

# Getting started

# Contributing

# Security

# Funding
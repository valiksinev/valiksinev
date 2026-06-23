# Valentin Sinev

**Rust developer at the intersection of Ethereum and Solana.**

> Author of **Rome EVM** — an Ethereum-equivalent execution layer running natively on Solana.
> Any Ethereum contract, tool, or wallet works unchanged, with the same semantics.

I work where the complexity is real: the full Solana stack — account-model
constraints, parallel execution, ALT, CPI, secure asset-vault design — and the
off-chain machinery that drives an on-chain EVM.

---

## 🔭 Rome EVM — what I built

At **Rome Protocol** I designed and built Rome EVM: the on-chain program, the
off-chain emulator, and the transaction sender.

The core problem: Solana's account model, transaction-size limits, and execution
constraints are fundamentally incompatible with Ethereum semantics. Rome EVM
bridges that gap without compromising EVM compatibility:

- **Iterative transaction execution** — splits long EVM runs across multiple
  Solana transactions, serializing full VM state between steps
- **Solana-native gas model** — gas accounting derived from Solana's own rules
- **Address Lookup Table integration** — for transactions touching large account sets
- **Custom heap allocator** — tuned for the on-chain execution environment
- **SBF emulator** — off-chain simulation of on-chain logic
- **Solidity ↔ CPI interface** — EVM bytecode can call native Solana programs directly

Result: MetaMask, ethers.js, Hardhat, and Foundry all work without modification.

🔗 **Rome EVM:**  · https://docs.rome.builders/

---

## 🛠 Tech

`Rust` · `Solana / SVM internals` · `EVM` · `Solidity` · `C / C++` · `Intel SGX` · `cryptography (BIP-32/39/44, transaction signing)`

---

## 💼 Experience

**Rome Protocol** — Core EVM Engineer · *2024 – present*
Architected and built Rome EVM (above).

**Neon Labs** — Rust Developer · *2021 – 2023*
Worked on Neon-EVM for Solana: transaction emulation inside the Solana BPF VM,
and the tracer-api service (EIP-1898 + Geth interfaces, trace collection,
historical-state execution). Implemented EIP-198 as a Solana node syscall
([solana#28503](https://github.com/solana-labs/solana/pull/28503)).

**oneFactor** — C++ Developer · *2019 – 2021*
Intel SGX service from scratch: remote/local enclave attestation, cryptographic scheme.

**Krypton Moscow** — C++ Developer · *2018 – 2019*
Key-storage & transaction-signing application
([array-io-keychain](https://github.com/arrayio/array-io-keychain)) — BIP-32/39/44
backup/restore, signing for Ethereum, Bitcoin, Bitshares.

*Earlier:* C developer in industrial automation and sensor firmware / signal
processing (2009 – 2017). Patent holder — *Glass Cleanliness Sensor*.

---

## 📫 Links

- GitHub: [github.com/valiksinev](https://github.com/valiksinev)
- LinkedIn: [linkedin.com/in/valentinesinev](https://www.linkedin.com/in/valentinesinev)
- Email: valik.sinev@gmail.com

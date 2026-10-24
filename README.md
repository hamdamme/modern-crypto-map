# Modern Crypto Map

A compact, source-linked map of cryptographic algorithms that were standardized recently or are still moving through standardization.

This repository is a learning guide, not an implementation or deployment recommendation. “Selected” and “under development” do not mean “final standard.”

## Recently finalized

| Algorithm family | What it does | Status |
| --- | --- | --- |
| **ML-KEM** (formerly CRYSTALS-Kyber) | Post-quantum key encapsulation: helps two parties establish a shared secret over a public channel. | Final NIST standard: [FIPS 203](https://csrc.nist.gov/pubs/fips/203/final), published August 2024. |
| **ML-DSA** (formerly CRYSTALS-Dilithium) | Post-quantum digital signatures. | Final NIST standard: [FIPS 204](https://csrc.nist.gov/pubs/fips/204/final), published August 2024. |
| **SLH-DSA** (based on SPHINCS+) | Stateless hash-based post-quantum digital signatures. | Final NIST standard: [FIPS 205](https://csrc.nist.gov/pubs/fips/205/final), published August 2024. |
| **Ascon** | Lightweight authenticated encryption, hashing, and extendable-output functions for constrained devices. | Final NIST standard: [SP 800-232](https://csrc.nist.gov/pubs/sp/800/232/final), published August 2025. |

## Selected or in development

| Algorithm | What it does | Current status |
| --- | --- | --- |
| **FN-DSA** (based on Falcon) | Post-quantum digital signatures. | Selected for standardization; [FIPS 206 is in development](https://csrc.nist.gov/Projects/Post-Quantum-Cryptography/Post-Quantum-Cryptography-Standardization). |
| **HQC** | Post-quantum key encapsulation, based on code-based cryptography. | Selected by NIST in March 2025 for standardization as a backup to ML-KEM; [the standard is still being developed](https://www.nist.gov/news-events/news/2025/03/nist-selects-hqc-fifth-algorithm-post-quantum-encryption). |

## New signature candidates

NIST advanced nine additional post-quantum signature candidates to a third evaluation round in May 2026. They remain candidates, not standards. NIST expects this evaluation phase to take about two years. The list and updates are on the [NIST project page](https://www.nist.gov/news-events/news/2026/05/nine-candidates-advance-third-round-additional-digital-signatures-pqc).

**Status note:** HAWK was later withdrawn from consideration in July 2026 after a reported mathematical vulnerability. It is not a recommended algorithm. See the update on the [NIST notice](https://www.nist.gov/news-events/news/2026/05/nine-candidates-advance-third-round-additional-digital-signatures-pqc).

## Quick distinctions

- **Key encapsulation** establishes shared secret material; it is commonly combined with symmetric encryption.
- **Digital signatures** authenticate a message or document and help detect modification.
- **Authenticated encryption** encrypts data and checks its integrity and authenticity.
- **Hashing** produces a fixed-size digest; a hash alone does not encrypt or authenticate data.

## Scope

This repo tracks algorithm families and their public standardization status. It does not contain cryptographic implementations, claim that any algorithm is unbreakable, or replace current standards and expert review.

Last reviewed: **2026-10-24**

## Sources

See [SOURCES.md](SOURCES.md) for the primary references used in this guide.

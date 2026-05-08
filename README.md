# ValiBlocks

**On-chain proof-of-existence for clinical trial and life sciences data.**

Clinical trials produce time-sensitive records that must remain demonstrably
unchanged from the moment of collection — patient measurements, observations,
adverse events. Regulators, sponsors, and patients all need confidence that
data recorded at a site today has not been altered, and that the timestamp
is trustworthy.

ValiBlocks provides that guarantee without requiring trust in any single
organisation.

---

## How it works

Your existing application hashes a data point locally using a standard
algorithm (SHA-256, SHA-3). Only the digest — never the underlying patient
data — is submitted to the smart contract. The contract records the digest
alongside the submitting address, the algorithm used, and a block timestamp.

To verify later: re-hash the same data and compare against the on-chain
record. If the digests match, the data is provably unchanged. No personal
or clinical data ever leaves your system.

---

## This repository

| Repository | Description |
|---|---|
| [val-chain](https://github.com/ValiBlocks/val-chain) | Core smart contracts, test suite, and integrator documentation |

---

## Who it's for

- **ePRO and EDC vendors** looking to add independently verifiable data
  integrity to their platform with minimal integration effort
- **Clinical trial sponsors** who need tamper-evident audit trails that
  don't rely on a single organisation's records
- **Regulators and auditors** who need to verify data integrity years after
  collection, without access to the original system

---

## Licensing

The smart contracts are source-available for review and self-audit.

**Commercial use requires a licence.** If you are a vendor or sponsor
interested in integrating ValiBlocks into a production system, contact us
to discuss commercial licensing terms.

📧 [info@valiblocks.com](mailto:info@valiblocks.com)

---

🌐 [valiblocks.com](https://valiblocks.com)

# Veritas Epoch Core ($VE)

> **"Data is a liability. Privacy is a right. Ephemerality is the solution."**

Veritas Epoch is a decentralized, privacy-preserving communication protocol forked from the **Monero (CryptoNote)** codebase. While traditional blockchains are designed to be "Immutable Ledgers of History," Veritas Epoch is engineered to be an **"Immutable Ledger of Truth, with a Finite Memory."**

---

## 1. Executive Summary
The digital age has a "bloat" problem. Every message sent on most blockchains exists forever, creating a permanent metadata trail and a massive storage burden for nodes. 

**Veritas Epoch** solves this by hardcoding a **15-day rolling window** into the consensus layer. After 15 days, the transaction "payload" (your encrypted message) is shredded by every node on the network. The financial integrity remains, but the data liability vanishes.

## 2. Core Technical Innovations

### A. The 15-Day "Shred-and-Store" Pulse
Unlike Monero's optional pruning, Veritas Epoch implements **Mandatory Protocol-Level Pruning**:
* **The Pulse:** Every 21,600 blocks (approx. 15 days), the network triggers a "payload purge."
* **Zero-Knowledge Erasure:** Nodes use a pruning algorithm that deletes the encrypted blob within a transaction while keeping the **Block Header** and **TX-Hash**. 
* **Integrity:** This ensures the $VE currency remains secure and spendable, but the *content* associated with the transaction is gone forever.

### B. "Fringe Mining" via RandomX
To ensure the network is secured by people, not server farms, we utilize the **RandomX Proof-of-Work** algorithm. 
* **Mobile-First:** Optimized for CPU-heavy mining. 
* **Onboarding Logic:** The **Vellum Chat** app features "Fringe Mining," where the device performs a brief mining burst during setup to earn the user their initial message credits without requiring an external exchange.

### C. The Vault (Future Milestone)
For users requiring persistence, we are developing **The Vault**: 
* A decentralized marketplace where users can pay $VE to "Archive Nodes."
* These nodes are incentivized to store encrypted data beyond the 15-day window via **Proof of Retrievability (PoR)** contracts.
* Utilizes **Private Information Retrieval (PIR)** to ensure the node cannot identify the data it is serving.

---

## 3. The 2025 Economic Model ($VE)
Veritas Epoch is built for longevity. To prevent the "Developer Burnout" that kills many open-source projects, we have hardcoded a **Sustainable Growth Split**:

| Allocation | Stakeholder | Purpose |
| :--- | :--- | :--- |
| **85%** | **Miners** | Securing the network and hosting the 15-day ledger. |
| **10%** | **Founder Wallet** | Perpetual royalty for the Architect to ensure long-term vision. |
| **5%** | **Dev Fund** | Managed by Multi-sig for third-party audits and core development. |

*This split applies to all block rewards and transaction fees in perpetuity.*

---

## 4. The Future: Vellum Chat & Beyond
Veritas Epoch is the engine; **Vellum** is the vehicle.

### Phase 1: The Pulse (Current)
* Finalizing the modification of `src/cryptonote_core` to automate payload deletion.
* Launching the Private Testnet for high-latency stress testing.

### Phase 2: Vellum Integration
* Release of the **Vellum Chat** mobile and desktop clients.
* Implementation of **Zero-Metadata** ID generation (no phones/emails).

### Phase 3: The Global Standard
* Expansion into **Corporate Integrity Tools**, allowing companies to use $VE for internal comms that automatically comply with 15-day data retention legal policies.
* Global node expansion to ensure sub-60-second message propagation.

---

## 🛡️ Vulnerability Response
We follow the Monero standard for responsible disclosure. Please contact **founder@veritasepoch.org** for any critical security findings. 

**Architect:** [EpochArchitect](https://github.com/epocharchitect)      
**Website:** [veritasepoch.org](https://veritasepoch.org)  
**App:** [vellum.chat](https://vellum.chat)

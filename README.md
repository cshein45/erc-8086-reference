# ERC-8086 — Native Privacy Token Standard (IZRC20)

ERC-8086 defines **IZRC20**, a minimal and extensible privacy interface for Ethereum.
This standard enables fully private asset transfers while remaining compatible with
existing ERC-20 infrastructure and tooling.

## Key Capabilities
- **Dual-Mode Tokens**: Public (ERC-20) + Private (ZRC-20) in a single system  
- **Wrapper Protocols**: Convert any token (e.g., DAI → zDAI → DAI)  
- **Native Privacy Layer**: Guarantees unlinkable transfers  
- **Auditable Logic**: Verifiers + proof system separated cleanly

---

## Ecosystem Stack (Standardized)

Ecosystem Stack:
┌─────────────────────────────────────┐
│  Applications (DeFi, DAO, Wallets)  │
├─────────────────────────────────────┤
│  Dual-Mode Tokens (ERC-20 + ZRC-20) │
│  Wrapper Protocols (ERC-20→ZRC-20)  │
├─────────────────────────────────────┤
│  IZRC20: Native Privacy Interface   │  ← ERC-8086 (core)
├─────────────────────────────────────┤
│  Ethereum L1 / L2s                  │
└─────────────────────────────────────┘

---

## Contract Structure

contracts/
│
├── interfaces/
│   ├── IZRC20.sol          # Core privacy interface (ERC-8086)
│   └── IVerifier.sol       # Verification interface
│
├── reference/
│   └── PrivacyToken.sol    # Minimal reference implementation
│
├── implementation/
│   └── PrivacyTokenFactory.sol  # Create privacy-wrapped tokens
│
└── deployments/
└── base-sepolia/       # Verified testnet deployments

---

## Reference Deployment

A verified testnet implementation is deployed on **Base Sepolia**.  
This allows developers to mint, wrap, and test private tokens instantly.

**Test App** (live):  
https://testnative.zkprotocol.xyz/

---

## Why ERC-8086 Matters

- Standardizes Ethereum privacy tokens  
- Ensures long-term backward compatibility  
- Fully composable with DeFi, DAO, and cross-chain protocols  
- Designed for L1, L2s, and modular rollup environments  
- Alignment with **Movement Privacy Standard v1**

---

## Movement Alignment (KoKyat Version)

ERC-8086 sits at **Layer 2 & 3** of the Movement Ecosystem Standard Alignment:

- Layer 2 → Token & Asset Layer (MOVE, zMOVE, wrappers)  
- Layer 3 → Identity & Privacy Reputation Layer  
- Fully compatible with MOVE Privacy Layer (pv1)  
- Easily integratable into Movement Wallet + DAO  
  
ERC-8086 = Movement Network privacy foundation.

━━━━━━━━━━━━━━━━━━


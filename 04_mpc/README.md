# 04 - ESSENTIAL Multi-Party Computation (MPC)

## Priority: ⭐⭐⭐ ESSENTIAL (if focusing on MPC)

## What is MPC?

**Multi-Party Computation** allows multiple parties to jointly compute a function on their private inputs without revealing those inputs to each other.

Example: Three companies want to know their average salary without revealing individual salaries to each other.

## Why MPC Matters

- **Privacy-preserving computation**: Compute on sensitive data without exposing it
- **Secure auctions**: Bid without revealing your bid to others
- **Threshold cryptography**: Split keys among parties, need k-of-n to use
- **Private set intersection**: Find common elements without revealing full sets
- **Federated learning**: Train ML models on private data

## Time Estimate

**4-6 weeks** for foundations (10-20 hours/week)

## Prerequisites

Before starting, you should have completed:
- ✅ **01_ESSENTIAL_Math_Foundations/** - Secret sharing uses polynomial math
- ✅ **02_ESSENTIAL_Crypto_Primitives/** - Commitments, OT uses crypto primitives
- ⚠️ **03_ESSENTIAL_Zero_Knowledge/** - Optional but helpful (ZK and MPC are related)

## What's in This Folder

### Folders:

1. **secret sharing/** (2 papers + Pedersen in root)
   - Shamir secret sharing
   - Verifiable secret sharing (VSS)
   - Pedersen commitments for VSS
   - Foundation of threshold cryptography

2. **oblivious transfer/** (10+ papers)
   - 1-out-of-2 OT
   - 1-out-of-n OT
   - OT extensions
   - Foundation of secure two-party computation

### Key Root Papers:

- **"Multiparty Computation with Faulty Majority (1990) - Beaver, Goldwasser"**
  - Foundational MPC paper
  - Shows feasibility of MPC

## Learning Path

### Week 1-2: Secret Sharing Foundations

**Goal**: Understand how to split secrets

**Read**:
1. ⭐⭐⭐ **"Non-Interactive and Information-Theoretic Secure Verifiable Secret Sharing [Pedersen Commitment Scheme]" (root folder)**
   - Shamir secret sharing
   - Pedersen commitments
   - Verifiable secret sharing (VSS)

2. ⭐⭐⭐ **"A Simple Publicly Verifiable Secret Sharing Scheme (1999) - Schoenmakers"** (in secret sharing/)

3. ⭐⭐⭐ **"Publicly Verifiable Secret Sharing (1996) - Stadler"** (in secret sharing/)

**Key Concepts**:
- Shamir's (t, n) threshold scheme
- Polynomial interpolation
- Dealer distributes shares
- Reconstruct with t+1 shares
- Verifiable secret sharing (VSS)
- Pedersen VSS

**Mathematics**:
- Secret s encoded as polynomial P(x): P(0) = s
- Share i is P(i)
- Any t+1 shares can reconstruct P (Lagrange interpolation)
- t or fewer shares reveal nothing (information-theoretic security)

**Self-Check**: Can you implement Shamir secret sharing?

**Hands-On**:
1. Implement (3, 5) Shamir secret sharing
2. Code Lagrange interpolation for reconstruction
3. Add Pedersen commitments for verification

**Why This Matters**:
- Foundation of threshold cryptography
- Used in distributed key generation
- Base layer for many MPC protocols

### Week 3-4: Oblivious Transfer

**Goal**: Understand OT - the fundamental MPC building block

**Read** (from oblivious transfer/):
1. ⭐⭐⭐ **"Equivalence Between Two Flavours of Oblivious Transfer (1987) - Crépeau"**
   - Foundational OT concepts

2. ⭐⭐⭐ **"Efficient Oblivious Transfer Protocols (2001) - Naor, Pinkas"**
   - Practical OT construction
   - Widely cited

3. ⭐⭐⭐ **"The Simplest Protocol for Oblivious Transfer (2015) - Chou, Orlandi"**
   - Modern, simple OT
   - Good for learning

4. ⭐⭐ **"Improved OT Extension for Transferring Short Secrets (2013)"**
   - OT extension (crucial for efficiency)

5. ⭐⭐ **"Faster Private Set Intersection based on OT Extension (2014)"**
   - Practical application of OT

**Key Concepts**:

**1-out-of-2 OT**:
- Sender has two messages: m₀, m₁
- Receiver has choice bit: b
- Receiver learns mᵦ only
- Sender learns nothing about b

**Properties**:
- Receiver privacy: Sender doesn't learn b
- Sender privacy: Receiver doesn't learn m_{1-b}
- Correctness: Receiver gets mᵦ

**OT Extension**:
- Use few "base" OTs to create many OTs cheaply
- Critical for practical MPC
- Reduces expensive public-key ops to cheap symmetric ops

**Self-Check**: Can you explain why OT is fundamental to secure two-party computation?

**Hands-On**:
1. Understand OT protocol flow
2. Use OT library (e.g., libOTe)
3. Implement simple OT-based protocol

**Why This Matters**:
- **Every** secure two-party computation can be built from OT
- Garbled circuits use OT for inputs
- Private set intersection uses OT
- Foundation of practical MPC

### Week 5-6: MPC Protocols & Applications

**Goal**: See how secret sharing and OT enable MPC

**Read**:
1. ⭐⭐⭐ **"Multiparty Computation with Faulty Majority (1990) - Beaver, Goldwasser"** (root folder)
   - General MPC feasibility
   - Security with dishonest majority

2. Look for garbled circuits papers in **03_ESSENTIAL_Zero_Knowledge/**:
   - "How to Garble Arithmetic Circuits (2012)"
   - "Faster Two-Party Computation Using Garbled Circuits (2013)"

3. Search root folder for additional MPC papers

4. ⭐⭐ OT application papers (private set intersection, etc.)

**Key Concepts**:

**MPC Paradigms**:
1. **Garbled Circuits** (Yao's protocol)
   - Two-party computation
   - One party "garbles" circuit
   - Other party evaluates using OT for inputs
   - Semi-honest security

2. **Secret Sharing Based**:
   - Additive/Shamir sharing
   - Each party holds share
   - Compute on shares
   - Can handle malicious parties

3. **Hybrid Approaches**:
   - SPDZ, MASCOT protocols
   - Combine secret sharing with commitments/MACs
   - Active security

**Security Models**:
- **Semi-honest (honest-but-curious)**: Follow protocol but try to learn more
- **Malicious**: Arbitrary deviations from protocol
- **Covert**: Malicious but fear detection

**Self-Check**: Can you explain the difference between garbled circuits and secret-sharing-based MPC?

**Why This Matters**:
- Real-world MPC uses these techniques
- Understand tradeoffs between approaches
- Foundation for implementing MPC systems

## Paper Reading Priority

### MUST READ:

1. ⭐⭐⭐ Pedersen VSS paper (root folder)
2. ⭐⭐⭐ Schoenmakers VSS paper (secret sharing/)
3. ⭐⭐⭐ Efficient Oblivious Transfer - Naor, Pinkas
4. ⭐⭐⭐ The Simplest Protocol for Oblivious Transfer
5. ⭐⭐⭐ Multiparty Computation with Faulty Majority

### STRONGLY RECOMMENDED:

6. ⭐⭐ OT Extension papers
7. ⭐⭐ Private Set Intersection papers
8. ⭐⭐ Garbled circuits papers (in ZK folder)
9. ⭐⭐ Publicly Verifiable Secret Sharing - Stadler

### ADVANCED:

10. ⭐ Adaptive Oblivious Transfer
11. ⭐ Attribute-based OT
12. ⭐ Advanced MPC protocols

## Key Concepts You Must Master

### Secret Sharing:
- ✅ Shamir (t, n) threshold schemes
- ✅ Polynomial interpolation (Lagrange)
- ✅ Information-theoretic security
- ✅ Verifiable secret sharing (VSS)
- ✅ Applications: threshold signatures, distributed key generation

### Oblivious Transfer:
- ✅ 1-out-of-2 OT definition and security
- ✅ 1-out-of-n OT
- ✅ OT extension concept
- ✅ Why OT is complete for secure computation
- ✅ Applications: garbled circuits, PSI

### MPC Foundations:
- ✅ Semi-honest vs. malicious security
- ✅ Garbled circuits approach
- ✅ Secret-sharing-based approach
- ✅ Real-world MPC tradeoffs

## Common Pitfalls

❌ **Don't**:
- Think MPC = encryption (it's much more!)
- Skip the math (polynomial interpolation is key)
- Ignore OT extension (real MPC is impossible without it)
- Assume MPC is always practical (communication costs can be high)

✅ **Do**:
- Understand the fundamental building blocks (SS + OT)
- Implement simple protocols to understand costs
- Learn about different security models
- Explore modern frameworks (MP-SPDZ, etc.)

## Hands-On Projects

### Beginner:
1. Implement Shamir (3, 5) secret sharing
2. Code polynomial interpolation
3. Use OT library for simple protocol

### Intermediate:
4. Build verifiable secret sharing with Pedersen commitments
5. Implement Yao's millionaires' problem with garbled circuits
6. Create private set intersection with OT

### Advanced:
7. Implement full Yao's garbled circuits protocol
8. Build threshold signature scheme
9. Create secure auction using MPC

## Libraries & Frameworks

### For Learning:
- **MP-SPDZ**: Multi-protocol MPC framework
- **EMP-toolkit**: Efficient multi-party protocols
- **libOTe**: Oblivious transfer library

### For Production:
- **MP-SPDZ**: Production-ready MPC
- **SCALE-MAMBA**: Secure computation with active security
- **Carbyne Stack**: Cloud-based MPC

### OT Libraries:
- **libOTe** (C++): Fast OT and OT extension
- **emp-ot** (C++): Part of EMP toolkit

## Connection to Other Topics

### Relation to Zero-Knowledge:
- MPC can be used to build ZK proofs
- Garbled circuits → ZK via cut-and-choose
- Secret sharing used in ZK protocols
- Complementary privacy techniques

### Relation to Threshold Cryptography:
- Secret sharing → Threshold signatures
- Distributed key generation uses VSS
- t-of-n signing without revealing key

### Relation to Blockchain:
- MPC for custody (no single key holder)
- Threshold ECDSA for wallets
- Private smart contracts

## MPC vs. ZK vs. FHE

**MPC**:
- Multiple parties, distributed computation
- Each party has private input
- Interactive (parties communicate)
- Good for: Auctions, voting, joint analytics

**Zero-Knowledge**:
- Prover convinces verifier
- One party proves to another
- Can be non-interactive
- Good for: Privacy-preserving authentication, scaling blockchains

**FHE**:
- Single party computes on encrypted data
- Data owner encrypts, cloud computes
- Non-interactive
- Good for: Cloud computation on private data

**Often combined**: MPC + ZK, MPC + FHE for different security goals

## Real-World Applications

1. **Privacy-Preserving Analytics**:
   - Companies jointly analyze data without sharing
   - Used in advertising, fraud detection

2. **Secure Auctions**:
   - Bid without revealing until winner determined
   - Used in government procurement

3. **Threshold Cryptography**:
   - Cryptocurrency wallets (no single key holder)
   - CA root key splitting

4. **Private Set Intersection**:
   - Find common contacts without revealing full lists
   - Used in contact tracing

5. **Federated Learning**:
   - Train ML models on private data
   - Medical research without sharing patient data

## Modern MPC Protocols (Beyond This Folder)

This folder covers foundations. Modern MPC includes:

- **SPDZ**: Secret-sharing with MACs (malicious security)
- **MASCOT**: OT-based preprocessing for SPDZ
- **ABY**: Combines arithmetic, Boolean, and Yao sharings
- **Overdrive**: Fast SPDZ preprocessing
- **TinyOT**: Efficient OT-based MPC

Explore these after mastering foundations.

## FAQ

**Q: Is MPC practical for real-world use?**
A: Yes! Modern MPC is efficient enough for many applications. OT extension and preprocessing make it feasible.

**Q: How does MPC relate to blockchain?**
A: MPC enables threshold signatures (no single key), private smart contracts, and decentralized custody.

**Q: Can MPC work with more than 2 parties?**
A: Yes! Secret-sharing-based MPC scales to many parties. Garbled circuits are primarily 2-party.

**Q: What's the communication cost?**
A: Significant. Parties must exchange many messages. This is the main bottleneck.

**Q: Semi-honest vs. malicious - which is used in practice?**
A: Malicious security is needed for real adversaries but costs more. Semi-honest is okay for non-adversarial settings.

## Self-Assessment

After finishing this folder, you should be able to:

✅ Implement Shamir secret sharing
✅ Explain oblivious transfer and why it's fundamental
✅ Understand OT extension concept
✅ Describe garbled circuits approach to MPC
✅ Explain secret-sharing-based MPC
✅ Compare semi-honest vs. malicious security
✅ Identify when to use MPC vs. ZK vs. FHE
✅ Use MPC libraries for simple protocols

## Next Steps

### If continuing MPC deep dive:
- Research SPDZ, MASCOT, ABY protocols
- Read recent MPC papers (2015+)
- Implement protocols using MP-SPDZ

### If moving to other topics:

**For FHE**:
→ [05_ESSENTIAL_FHE_and_Lattices/README.md](../05_ESSENTIAL_FHE_and_Lattices/README.md)

**For applications**:
→ [06_IMPORTANT_Applications/README.md](../06_IMPORTANT_Applications/README.md)

## Additional Resources

### Books:
- "A Pragmatic Introduction to Secure Multi-Party Computation" - Evans et al. (free online)
- "Secure Multiparty Computation and Secret Sharing" - Cramer et al.

### Online Courses:
- Dan Boneh's Applied Cryptography (includes MPC)
- MIT 6.875 Cryptography (MPC sections)

### Tutorials:
- MP-SPDZ documentation and tutorials
- EMP-toolkit examples
- MPC Study Group resources

### Communities:
- IACR ePrint (search "multiparty computation")
- MPC Alliance
- Real World Crypto conference

---

**Remember**: MPC is about enabling multiple parties to compute together while keeping data private. Secret sharing and oblivious transfer are your fundamental building blocks.

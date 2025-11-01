# ZK-Library Beginner's Guide

**Purpose**: This guide helps beginners identify which folders and papers are essential, important, advanced, or irrelevant for learning Zero-Knowledge Proofs, Cryptography, FHE, MPC, and Security Enclaves.

**Goal**: After reading the recommended papers, you should be able to understand, write, and prove zero-knowledge systems.

---

## Legend

- **ESSENTIAL** ⭐⭐⭐ - Must read for beginners. Core foundations.
- **IMPORTANT** ⭐⭐ - Read after essentials. Builds critical knowledge.
- **ADVANCED** ⭐ - Read later. Requires deep understanding of essentials.
- **SPECIALIZED** 🔧 - Niche topics. Read only if specifically interested.
- **IRRELEVANT** ❌ - Skip for now. Not needed for ZK/crypto fundamentals.

---

## Core Learning Path

### Phase 1: Mathematical Foundations (Start Here)

#### 1. **number theory/** - ⭐⭐⭐ ESSENTIAL
- **Papers**: 9 papers
- **Why Essential**: Number theory is the foundation of all cryptography. You cannot understand ZK, FHE, or MPC without it.
- **Key Concepts**: Primes, modular arithmetic, discrete logarithm problem
- **Read First**: Papers on basic number theory, prime numbers
- **Priority**: HIGH - Start here before anything else

#### 2. **algebra/** - ⭐⭐⭐ ESSENTIAL
- **Papers**: 6 papers
- **Why Essential**: Group theory, rings, and fields are fundamental to understanding cryptographic protocols
- **Key Concepts**: Groups, rings, fields, finite fields
- **Priority**: HIGH - Read alongside number theory

#### 3. **Handbook of Applied Cryptography/** - ⭐⭐⭐ ESSENTIAL
- **Papers**: 19 chapters/papers
- **Why Essential**: Comprehensive introduction to cryptography. Standard reference.
- **Priority**: HIGH - Your cryptography bible

---

### Phase 2: Core Cryptographic Primitives

#### 4. **elliptic curve cryptography/** - ⭐⭐⭐ ESSENTIAL
- **Papers**: 28 papers
- **Why Essential**: Modern ZK systems (SNARKs, STARKs) heavily use elliptic curves and pairings
- **Key Concepts**: EC operations, point arithmetic, EC-based protocols
- **Note**: Critical for understanding pairing-based ZK systems
- **Priority**: HIGH - Essential for modern ZK

#### 5. **pairing-based cryptography/** - ⭐⭐⭐ ESSENTIAL
- **Papers**: 9 papers
- **Why Essential**: Most modern ZK-SNARKs use bilinear pairings
- **Key Concepts**: Bilinear maps, pairing-friendly curves
- **Dependency**: Read after elliptic curves
- **Priority**: HIGH - Core to zkSNARKs (Groth16, etc.)

#### 6. **hashes/** - ⭐⭐ IMPORTANT
- **Papers**: 9 papers
- **Why Important**: Used in commitment schemes, Merkle trees, and some ZK systems
- **Key Concepts**: Collision resistance, hash functions, commitments
- **Priority**: MEDIUM-HIGH

#### 7. **signature schemes/** - ⭐⭐ IMPORTANT
- **Papers**: 12 papers
- **Why Important**: Understanding signatures helps with ZK identification protocols
- **Key Concepts**: Digital signatures, Schnorr, ECDSA
- **Priority**: MEDIUM

---

### Phase 3: Zero-Knowledge Foundations (CORE)

#### 8. **zero knowledge/** - ⭐⭐⭐ ESSENTIAL (PRIMARY FOCUS)
- **Papers**: 30+ papers (including subfolders)
- **Why Essential**: THIS IS YOUR MAIN FOCUS. Everything builds toward this.
- **Must Read Papers**:
  - "Zero-Knowledge Proofs (2016) [lecture] - Miller.pdf" - START HERE
  - "Proofs that yield nothing but their validity..." (1991) - Goldreich, Micali, Wigderson - FOUNDATIONAL
  - "Efficient Identification and Signatures for Smart Cards (1989) - Schnorr" - Sigma protocols
  - "A Graduate Course in Applied Cryptography (2017) - Boneh, Shoup" - Comprehensive
- **Subfolders**:
  - **zkSNARKs/** - ⭐⭐⭐ ESSENTIAL - Must understand for modern ZK
  - **range proofs/** - ⭐⭐ IMPORTANT - Practical ZK applications
- **Priority**: HIGHEST - This is your destination

---

### Phase 4: MPC & Related Protocols

#### 9. **secret sharing/** - ⭐⭐⭐ ESSENTIAL for MPC
- **Papers**: 2 papers (+ Pedersen in root)
- **Why Essential**: Foundation of MPC protocols
- **Key Papers**:
  - "Non-Interactive and Information-Theoretic Secure Verifiable Secret Sharing [Pedersen Commitment Scheme]" (root folder)
  - Papers in secret sharing folder
- **Priority**: HIGH for MPC understanding

#### 10. **oblivious transfer/** - ⭐⭐⭐ ESSENTIAL for MPC
- **Papers**: 10+ papers
- **Why Essential**: Core building block for MPC and secure computation
- **Key Concepts**: OT protocols, OT extensions
- **Priority**: HIGH for MPC

#### 11. Find MPC papers in root and other folders
- Look for "Multiparty Computation" papers in root directory
- **Priority**: HIGH - Critical for MPC understanding

---

### Phase 5: Advanced Cryptographic Systems

#### 12. **fully homomorphic encryption/** - ⭐⭐⭐ ESSENTIAL for FHE
- **Papers**: 1 foundational paper
- **Key Paper**: "A Fully Homomorphic Encryption Scheme [Thesis] (2009) - Gentry.pdf"
- **Why Essential**: THE paper that started FHE. Must read for FHE understanding.
- **Warning**: Very advanced. Read after strong foundation in lattices.
- **Priority**: HIGH (if focusing on FHE)

#### 13. **lattice-based cryptography/** - ⭐⭐⭐ ESSENTIAL for FHE
- **Papers**: 22 papers
- **Why Essential**: FHE is built on lattice assumptions. Post-quantum security.
- **Key Concepts**: LWE, Ring-LWE, lattice problems
- **Dependency**: Critical for understanding FHE (Gentry's construction)
- **Priority**: HIGH for FHE, post-quantum crypto

#### 14. **post-quantum cryptography/** - ⭐⭐ IMPORTANT
- **Papers**: 21 papers
- **Why Important**: Future-proof cryptography. Overlaps with lattices.
- **Priority**: MEDIUM (unless focusing on PQC)

---

### Phase 6: Practical Applications

#### 15. **cryptocurrencies/** - ⭐⭐ IMPORTANT
- **Papers**: 12 papers
- **Why Important**: Real-world ZK applications (Zerocash, Zcash, Monero)
- **Key Papers**:
  - "Zerocash: Decentralized Anonymous Payments from Bitcoin"
  - "CryptoNote v2.0" (Monero)
- **Priority**: MEDIUM - Great for seeing ZK in practice

#### 16. **anonymous credentials/** - ⭐⭐ IMPORTANT
- **Papers**: 20 papers
- **Why Important**: Practical applications of ZK proofs
- **Priority**: MEDIUM - Read after ZK foundations

---

## IRRELEVANT or LOW PRIORITY for ZK/FHE/MPC Beginners

### ❌ Skip These Folders Initially

#### 17. **side channels/** - ❌ IRRELEVANT for theoretical understanding
- **Papers**: 26 papers
- **Why Skip**: Implementation security, not cryptographic foundations
- **When to Read**: Only when implementing real systems
- **Priority**: SKIP for now

#### 18. **visual cryptography/** - ❌ IRRELEVANT
- **Papers**: 2 papers
- **Why Skip**: Niche topic, not related to ZK/FHE/MPC
- **Priority**: SKIP entirely

#### 19. **knot theory/** - ❌ IRRELEVANT
- **Papers**: 4 papers
- **Why Skip**: Experimental cryptography, not mainstream
- **Priority**: SKIP entirely

#### 20. **quaternions/** - 🔧 SPECIALIZED
- **Papers**: 3 papers
- **Why Skip**: Very niche, not needed for ZK/FHE/MPC
- **Priority**: SKIP unless specifically interested

#### 21. **hyperelliptic/** - 🔧 SPECIALIZED
- **Papers**: 6 papers
- **Why Skip**: Alternative to elliptic curves, not commonly used in ZK
- **Priority**: LOW - Only for specialists

#### 22. **camellia/** - ❌ IRRELEVANT
- **Papers**: 1 paper
- **Why Skip**: Specific block cipher, not needed for ZK
- **Priority**: SKIP

#### 23. **differential cryptanalysis/** - 🔧 SPECIALIZED
- **Papers**: 2 papers
- **Why Skip**: Cryptanalysis technique, not needed for building ZK
- **Priority**: LOW

#### 24. **elgamal/** - ⭐ ADVANCED (but not critical)
- **Papers**: 2 papers
- **Why Limited**: Good to know, but not essential for modern ZK
- **Priority**: LOW-MEDIUM

#### 25. **otr/** - 🔧 SPECIALIZED
- **Papers**: 7 papers
- **Why Skip**: Off-the-Record messaging protocol, specific application
- **Priority**: SKIP for ZK focus

#### 26. **patents/** - ❌ IRRELEVANT
- **Papers**: 1 paper
- **Why Skip**: Legal documents, not technical learning
- **Priority**: SKIP

#### 27. **standards/** - ⭐ ADVANCED
- **Papers**: 4 papers
- **Why Later**: Implementation standards, read after understanding concepts
- **Priority**: LOW initially

#### 28. **formal verification/** - ⭐ ADVANCED
- **Papers**: 1 paper
- **Why Later**: Advanced topic for proving correctness
- **Priority**: LOW initially

#### 29. **quantum algorithms & cryptanalysis/** - 🔧 SPECIALIZED
- **Papers**: 2 papers
- **Why Skip**: Unless focusing on quantum computing
- **Priority**: LOW (unless quantum focus)

#### 30. **quantum cryptography/** - 🔧 SPECIALIZED
- **Papers**: 8 papers
- **Why Skip**: Different paradigm (QKD), not related to ZK/FHE
- **Priority**: LOW (unless quantum focus)

#### 31. **isogeny-based cryptography/** - ⭐ ADVANCED
- **Papers**: 1 paper
- **Why Later**: Advanced post-quantum crypto
- **Priority**: LOW

#### 32. **supersingular isogeny/** - ⭐ ADVANCED
- **Papers**: 4 papers
- **Why Later**: Advanced topic, post-quantum
- **Priority**: LOW

#### 33. **rank-based cryptography/** - ⭐ ADVANCED
- **Papers**: 1 paper
- **Why Later**: Experimental post-quantum approach
- **Priority**: LOW

---

### MODERATE PRIORITY (Read After Core Topics)

#### 34. **authenticated encryption/** - ⭐⭐ IMPORTANT
- **Papers**: 10 papers
- **Why Important**: Practical crypto, but not core to ZK theory
- **Priority**: MEDIUM

#### 35. **block ciphers/** - ⭐⭐ IMPORTANT
- **Papers**: 4 papers
- **Why Important**: Understanding symmetric crypto helps, but not core to ZK
- **Priority**: MEDIUM

#### 36. **stream ciphers/** - ⭐ ADVANCED
- **Papers**: 3 papers
- **Why Later**: Less relevant to ZK/FHE/MPC
- **Priority**: LOW-MEDIUM

#### 37. **random number generators/** - ⭐⭐ IMPORTANT
- **Papers**: 5 papers
- **Why Important**: Important for implementations, not theory
- **Priority**: MEDIUM

#### 38. **rsa/** - ⭐⭐ IMPORTANT
- **Papers**: 6 papers
- **Why Important**: Classic crypto, good foundation, but not used in modern ZK
- **Priority**: MEDIUM

#### 39. **ibe/** (Identity-Based Encryption) - ⭐ ADVANCED
- **Papers**: 5 papers
- **Why Later**: Advanced topic, uses pairings but not core to ZK
- **Priority**: LOW-MEDIUM

#### 40. **attribute-based encryption/** - ⭐ ADVANCED
- **Papers**: 1 paper
- **Why Later**: Advanced topic, not core to ZK
- **Priority**: LOW

#### 41. **private information retrieval/** - 🔧 SPECIALIZED
- **Papers**: 3 papers
- **Why Specialized**: Related to MPC but niche
- **Priority**: LOW-MEDIUM (higher if MPC focus)

#### 42. **security models/** - ⭐⭐ IMPORTANT
- **Papers**: 1 paper
- **Why Important**: Understanding security definitions is important
- **Priority**: MEDIUM

---

## Root Folder Papers (~/zk-library/*.pdf)

**132 papers in root** - Mixed relevance. Key papers:

### ESSENTIAL Root Papers:
- "A Graduate Course in Applied Cryptography (2017) - Boneh, Shoup" - ⭐⭐⭐
- "Cryptography Made Simple (2016) - Smart" - ⭐⭐⭐
- "Non-Interactive and Information-Theoretic Secure Verifiable Secret Sharing [Pedersen Commitment Scheme]" - ⭐⭐⭐
- "Zerocash: Decentralized Anonymous Payments from Bitcoin" - ⭐⭐

### IMPORTANT Root Papers:
- "Cryptographic Sponge Functions" - ⭐⭐ (for hash-based ZK)
- Papers on commitments, blind signatures - ⭐⭐
- E-cash papers (practical ZK applications) - ⭐⭐

### SKIP in Root:
- NSA/GCHQ documents - ❌ (historical interest only)
- "Mathematics Made Difficult" - ❌ (satirical)
- Specific protocol papers until you need them - ⭐

---

## Special Folders

### 43. **crypto_conferences/** - 🔧 REFERENCE
- Conference proceedings
- **Use**: Reference when you need specific papers
- **Priority**: SKIP for linear reading, use as needed

### 44. **Rethinking Public Key Infrastructures.../** - ⭐⭐ IMPORTANT
- **Papers**: 15 papers
- **Focus**: Privacy-preserving PKI, credential systems
- **Priority**: MEDIUM (after ZK foundations)

---

## Recommended Reading Order

### Beginner Path (3-6 months):

1. **Mathematical Foundations** (2-4 weeks)
   - number theory/
   - algebra/
   - Relevant chapters from Handbook of Applied Cryptography

2. **Core Cryptography** (4-6 weeks)
   - elliptic curve cryptography/ (basics)
   - hashes/
   - signature schemes/ (Schnorr especially)

3. **Zero-Knowledge Fundamentals** (8-12 weeks)
   - zero knowledge/ - READ EVERYTHING
   - Start with Miller's lecture notes
   - Goldreich-Micali-Wigderson paper
   - Schnorr protocols
   - Work through zkSNARKs subfolder

4. **Pairings for ZK** (2-3 weeks)
   - pairing-based cryptography/
   - Groth-Sahai proofs
   - Pairing-based SNARKs

### MPC Focus (add 2-3 months):

5. **MPC Foundations**
   - secret sharing/
   - oblivious transfer/
   - Garbled circuits papers in zero knowledge/
   - Root papers on MPC

### FHE Focus (add 3-4 months):

6. **Lattices & FHE**
   - lattice-based cryptography/ (basics first)
   - fully homomorphic encryption/ (Gentry's thesis)
   - post-quantum cryptography/ (LWE-based schemes)

### Advanced (6-12 months later):

7. **Applications & Advanced Topics**
   - cryptocurrencies/ (Zerocash, Monero)
   - anonymous credentials/
   - authenticated encryption/
   - private information retrieval/

---

## Security Enclaves Note

**No dedicated folder for security enclaves** (SGX, TrustZone, etc.)

Security enclaves are **hardware-based trusted execution environments**, which is a different paradigm from cryptographic protocols. For enclaves:
- Focus on understanding trusted computing
- Read about Intel SGX, ARM TrustZone separately
- Understand how ZK can complement or replace enclave trust assumptions
- Some root papers may discuss attestation and trusted hardware

**Recommendation**: Learn ZK/crypto foundations first, then study enclaves from separate resources.

---

## Quick Start (Absolute Beginner)

If you're completely new and overwhelmed:

### Week 1-2: Prerequisites
1. Read basic number theory primer
2. Skim "Handbook of Applied Cryptography" - Chapters 1-3

### Week 3-4: First ZK Paper
3. Read "Zero-Knowledge Proofs (2016) [lecture] - Miller.pdf"

### Week 5-8: Core Concepts
4. Read Schnorr identification protocol
5. Read "Proofs that yield nothing but their validity" (GMW)
6. Understand Sigma protocols

### Week 9-12: Modern ZK
7. Start zkSNARKs/ subfolder
8. Read about Groth16, PLONK fundamentals

### Month 4+: Specialize
9. Choose: SNARKs, STARKs, FHE, or MPC
10. Deep dive into relevant folders

---

## Summary Table

| Folder | Priority | Relevance | When to Read |
|--------|----------|-----------|--------------|
| number theory | ⭐⭐⭐ | ESSENTIAL | Week 1-2 |
| algebra | ⭐⭐⭐ | ESSENTIAL | Week 1-2 |
| Handbook of Applied Cryptography | ⭐⭐⭐ | ESSENTIAL | Week 1-4 |
| elliptic curve cryptography | ⭐⭐⭐ | ESSENTIAL | Week 3-6 |
| pairing-based cryptography | ⭐⭐⭐ | ESSENTIAL | Week 6-8 |
| **zero knowledge** | ⭐⭐⭐ | **ESSENTIAL** | **Week 3-16+** |
| secret sharing | ⭐⭐⭐ | ESSENTIAL (MPC) | Week 6-8 |
| oblivious transfer | ⭐⭐⭐ | ESSENTIAL (MPC) | Week 8-10 |
| lattice-based cryptography | ⭐⭐⭐ | ESSENTIAL (FHE) | Month 3-4 |
| fully homomorphic encryption | ⭐⭐⭐ | ESSENTIAL (FHE) | Month 4-6 |
| hashes | ⭐⭐ | IMPORTANT | Week 2-4 |
| signature schemes | ⭐⭐ | IMPORTANT | Week 4-6 |
| cryptocurrencies | ⭐⭐ | IMPORTANT | Month 4+ |
| anonymous credentials | ⭐⭐ | IMPORTANT | Month 4+ |
| post-quantum cryptography | ⭐⭐ | IMPORTANT | Month 3+ |
| authenticated encryption | ⭐⭐ | IMPORTANT | Month 2-3 |
| side channels | ❌ | SKIP | When implementing |
| visual cryptography | ❌ | SKIP | Never (for ZK) |
| knot theory | ❌ | SKIP | Never (for ZK) |
| quaternions | 🔧 | SPECIALIZED | If interested |
| quantum cryptography | 🔧 | SPECIALIZED | If interested |

---

## Final Recommendations

### DO READ (Priority Order):
1. **zero knowledge/** - Your main destination
2. **number theory/** & **algebra/** - Your foundation
3. **elliptic curve cryptography/** - Modern ZK uses this
4. **pairing-based cryptography/** - zkSNARKs need this
5. **lattice-based cryptography/** - For FHE and post-quantum
6. **secret sharing/** & **oblivious transfer/** - For MPC
7. **Handbook of Applied Cryptography/** - Your reference

### DON'T READ (Until Much Later):
- side channels, visual cryptography, knot theory, quaternions
- camellia, otr, patents, standards (initially)
- Most quantum topics (unless that's your focus)
- Specialized post-quantum schemes (isogeny, rank-based)

### MAYBE READ (Based on Interest):
- cryptocurrencies (great motivation and applications)
- anonymous credentials (practical ZK)
- random number generators, block ciphers (implementation)
- formal verification (proving correctness)

---

## Additional Resources Needed

This library is excellent but missing some beginner-friendly content:

### Suggested External Resources:
1. **Online Courses**:
   - Dan Boneh's Cryptography courses (Coursera)
   - zkSNARKs MOOC
2. **Tutorials**:
   - ZK proofs from scratch tutorials
   - Circom/SnarkJS practical guides
3. **Books**:
   - "Introduction to Modern Cryptography" - Katz & Lindell
4. **Security Enclaves**:
   - Intel SGX documentation
   - ARM TrustZone guides
   - Papers on TEE security models

---

**Last Updated**: 2025-11-01
**Maintainer**: Add your name/contact
**Contributions**: Please update as you discover essential/irrelevant papers

---

## How to Use This Guide

1. **Complete Beginner**: Follow "Quick Start" section, then "Recommended Reading Order"
2. **Some Crypto Background**: Skip to Phase 3 (Zero-Knowledge Foundations)
3. **Focused on FHE**: Read foundations (Phase 1-2), then jump to lattice + FHE
4. **Focused on MPC**: Read foundations, then secret sharing + oblivious transfer
5. **Implementing ZK Systems**: Focus on zero knowledge/ + elliptic curves + pairings

Remember: **Quality over quantity**. Better to deeply understand 20 essential papers than to skim 200.

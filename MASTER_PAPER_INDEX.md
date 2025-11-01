# Master Paper Index - ZK Library

This comprehensive index catalogs **all 600+ papers** in this library with priority ratings, difficulty levels, and learning recommendations.

**Last Updated**: 2025-01-01

---

## How to Use This Index

### Priority Ratings

- ⭐⭐⭐ **MUST READ** - Essential for understanding the field
- ⭐⭐ **RECOMMENDED** - Important for deeper understanding
- ⭐ **OPTIONAL** - Specialized topics or advanced research

### Difficulty Levels

- 🟢 **Beginner** - Accessible with basic crypto knowledge
- 🟡 **Intermediate** - Requires solid foundation (folders 01-02)
- 🔴 **Advanced** - Requires expertise in multiple areas
- ⚫ **Expert** - Cutting-edge research, highly specialized

### Reading Order

- 📖 **Linear** - Read in suggested order
- 🔀 **Flexible** - Can be read independently
- 🔄 **Prerequisite** - Must read before other papers

---

## Table of Contents

1. [01 - Math Foundations](#01---essential-math-foundations)
2. [02 - Cryptographic Primitives](#02---essential-cryptographic-primitives)
3. [03 - Zero-Knowledge Proofs](#03---essential-zero-knowledge-proofs)
4. [04 - Multiparty Computation](#04---essential-multiparty-computation)
5. [05 - FHE and Lattices](#05---essential-fhe-and-lattices)
6. [06 - Applications](#06---important-applications)
7. [07 - Advanced Topics](#07---advanced-topics)
8. [Recently Added Papers](#recently-added-papers-from-root-directory)
9. [Papers to Download](#papers-to-download-2018-2025)

---

## 01 - Essential Math Foundations

**Total Papers**: ~40+ papers
**Time Estimate**: 4-8 weeks
**Priority**: 🔄 Prerequisite for everything else

### Number Theory

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| Prime Numbers and Computer Methods for Factorization (1994/2012) - Riesel | ⭐⭐⭐ | 🟡 | Comprehensive factorization reference |
| Introduction to Twin Primes and Brun's Constant | ⭐ | 🟢 | Interesting but not critical |
| What is the smallest prime? (2012) | ⭐ | 🟢 | Conceptual discussion |
| Detecting Perfect Powers in Essentially Linear Time - Bernstein | ⭐⭐ | 🔴 | Algorithmic number theory |
| The Number Field Sieve for Integers of Low Weight (2010) | ⭐⭐ | 🔴 | Advanced factorization |

### Algebra & Computational Algebra

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| Ideals, Varieties, and Algorithms (2015) - Cox, Little, O'Shea | ⭐⭐⭐ | 🟡 | **Essential** for understanding algebraic crypto |
| Gröbner Bases, Coding, and Cryptography (2009) | ⭐⭐ | 🔴 | Important for MQ cryptography |
| Geometric Algebra with Applications | ⭐ | 🟡 | Alternative algebraic framework |
| Inner Product Spaces (2007) | ⭐⭐ | 🟢 | Foundation for lattice crypto |

### Finite Fields

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| Finite Fields - Lange | ⭐⭐⭐ | 🟡 | **Must read** - Concise and clear |
| Finite Fields with Applications (2010) | ⭐⭐⭐ | 🟡 | Comprehensive reference |

### Textbooks

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| An Introduction to Mathematical Cryptography (2014) - Hoffstein, Pipher, Silverman | ⭐⭐⭐ | 🟡 | **Start here** - Best intro textbook |
| Handbook of Applied Cryptography (19 chapters) | ⭐⭐⭐ | 🟡 | **Reference bible** - Keep handy |

---

## 02 - Essential Cryptographic Primitives

**Total Papers**: ~100+ papers
**Time Estimate**: 6-10 weeks
**Priority**: 🔄 Prerequisite for ZK and advanced topics

### Textbooks

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| Cryptography Made Simple (2016) - Smart | ⭐⭐⭐ | 🟡 | **Excellent** modern textbook |
| Cryptography and Coding (2005) - Smart | ⭐⭐ | 🔴 | Conference proceedings |

### Elliptic Curve Cryptography

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| Faster Point Multiplication (2001) - Gallant, Lambert, Vanstone | ⭐⭐⭐ | 🟡 | GLV method - widely used |
| Batch Binary Edwards (2009) - Bernstein | ⭐⭐ | 🔴 | Edwards curves optimization |
| Kummer Strikes Back (2014) - Bernstein, Lange, et al. | ⭐⭐ | 🔴 | Fastest Diffie-Hellman |
| Modular Polynomials via Isogeny Volcanoes (2012) | ⭐⭐ | ⚫ | Advanced isogeny theory |
| New Algorithm for DLP on Elliptic Curves (2015) - Semaev | ⭐⭐ | 🔴 | Security analysis |
| Short Programs for Functions on Curves (1986) - Miller | ⭐⭐⭐ | 🔴 | **Miller's algorithm** for pairings |
| Rational Curves on K3 Surface (2009) - Elkies | ⭐ | ⚫ | Advanced algebraic geometry |

### Pairing-Based Cryptography

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| All papers in `pairing-based cryptography/` folder | ⭐⭐⭐ | 🟡 | **Essential** for zkSNARKs |

### Hash Functions

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| Cryptographic Sponge Functions (2011) - Keccak team | ⭐⭐⭐ | 🟡 | Foundation of SHA-3 |
| Papers in `hashes/keccak/`, `hashes/sha1/`, etc. | ⭐⭐ | 🟢-🟡 | Understanding modern hashes |

### Message Authentication

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| The Poly1305-AES MAC (2005) - Bernstein | ⭐⭐⭐ | 🟡 | Used in TLS 1.3 |
| Polynomial Evaluation and Message Authentication (2007) - Bernstein | ⭐⭐ | 🟡 | Theory behind Poly1305 |
| Message Authentication, Revisited (2012) | ⭐⭐ | 🔴 | Modern security analysis |

### Stream Ciphers

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| A Security Analysis of ChaCha20 and Poly1305 (2014) | ⭐⭐⭐ | 🟡 | **Modern standard** (TLS 1.3) |
| Extending the Salsa20 Nonce (2011) - Bernstein | ⭐⭐ | 🟡 | XSalsa20 construction |

### Discrete Log Attacks

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| A Key Recovery Attack on Discrete Log (1997) - Lim, Lee | ⭐⭐ | 🟡 | Small subgroup attacks |
| A Kilobit Hidden SNFS Discrete Log (2016) | ⭐⭐ | 🔴 | Large-scale DLP computation |
| The Decision Diffie-Hellman Problem (1998) - Boneh | ⭐⭐⭐ | 🟡 | **DDH assumption** essential |
| Imperfect Forward Secrecy: DH Fails in Practice (2015) | ⭐⭐⭐ | 🟡 | **Logjam attack** - practical security |
| Mining Your Ps and Qs (2012) - Heninger et al. | ⭐⭐⭐ | 🟢 | **Fascinating** RSA key analysis |
| Extended Tower Number Field Sieve (2016) | ⭐⭐ | ⚫ | Cutting-edge DLP algorithms |

### Signature Schemes

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| Batch Verification of Short Signatures (2011) - Camenisch et al. | ⭐⭐⭐ | 🟡 | Efficient signature batching |
| Faster Batch Forgery Identification (2012) - Bernstein et al. | ⭐⭐ | 🔴 | Security enhancement |
| Fiat-Shamir Transform paper (2002) - Bellare et al. | ⭐⭐⭐ | 🟡 | **Critical** for ZK proofs |
| Two-Party Generation of DSA Signatures (2001) | ⭐⭐ | 🔴 | Threshold signatures |
| Group Signature with Deniability (2015) | ⭐ | 🔴 | Privacy-preserving signatures |
| Extensions to Chaum's Blind Signature Scheme | ⭐⭐ | 🟡 | Foundation of e-cash |

---

## 03 - Essential Zero-Knowledge Proofs

**Total Papers**: 35+ papers (now expanded)
**Time Estimate**: 8-16 weeks
**Priority**: ⭐⭐⭐ **YOUR DESTINATION**

### Foundational ZK Papers (Main Folder)

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| Zero-Knowledge Proofs (2016) [lecture] - Miller | ⭐⭐⭐ | 🟢 | **START HERE** - Best introduction |
| Proofs that yield nothing but their validity (1991) - GMW | ⭐⭐⭐ | 🔴 | **THE foundational paper** |
| Efficient Identification for Smart Cards (1989) - Schnorr | ⭐⭐⭐ | 🟢 | **Schnorr protocol** - essential |
| Zero-Knowledge Proofs of Identity (1988) - Fiat, Shamir | ⭐⭐⭐ | 🟡 | **Fiat-Shamir** heuristic |
| Proof Systems for General Statements (1997) - Camenisch, Stadler | ⭐⭐⭐ | 🟡 | **Sigma protocols** |
| A Graduate Course in Applied Cryptography - Boneh, Shoup | ⭐⭐⭐ | 🟡 | **Modern reference** |

### Groth-Sahai Proofs (NEW SUBFOLDER!)

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| Efficient Non-interactive Proof Systems for Bilinear Groups (2008) - Groth, Sahai | ⭐⭐⭐ | 🔴 | **FOUNDATION** of modern zkSNARKs |
| Efficient Non-interactive Proof Systems [full] (2008) | ⭐⭐⭐ | ⚫ | Complete version with all proofs |

### Commitment Schemes (NEW SUBFOLDER!)

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| Non-Interactive and IT-Secure Verifiable Secret Sharing [Pedersen] (1989) | ⭐⭐⭐ | 🟡 | **Pedersen commitments** - essential |
| Homomorphic Trapdoor Commitments (2009) - Groth | ⭐⭐ | 🔴 | Advanced commitment constructions |
| Structure Preserving Signatures and Commitments (2010) | ⭐⭐ | 🔴 | Connects signatures to ZK |

### NIZK (NEW SUBFOLDER! - Conference Papers)

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| Unconditional Characteristics of NIZK (2005) | ⭐⭐⭐ | 🔴 | Foundational NIZK theory |
| Non-interactive Zaps and New Techniques (2006) | ⭐⭐⭐ | 🔴 | Important NIZK constructions |
| On Signatures of Knowledge (2006) | ⭐⭐ | 🟡 | Connects signatures to ZK |
| Zero-Knowledge from Secure MPC (2007) | ⭐⭐ | 🔴 | Connecting ZK and MPC |

### zkSNARKs Subfolder

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| Succinct Non-Interactive ZK for von Neumann (2014) - Ben-Sasson et al. | ⭐⭐⭐ | 🔴 | **Foundation** of zkSNARKs |
| SNARKs for C (2013) - Ben-Sasson et al. | ⭐⭐⭐ | 🔴 | Practical zkSNARKs |
| QAP and Succinct NIZKs without PCPs (2014) - Gennaro et al. | ⭐⭐⭐ | 🔴 | **QAP construction** |
| Succinct NIAs via Linear Interactive Proofs (2013) - Bitansky et al. | ⭐⭐ | ⚫ | Theoretical foundations |

### Range Proofs Subfolder

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| Efficient Protocols for Set Membership and Range Proofs (2008) | ⭐⭐⭐ | 🟡 | **Classical** range proofs |
| Borromean Ring Signatures (2015) | ⭐⭐ | 🟡 | Related construction |
| Additional range proof papers | ⭐⭐ | 🟡-🔴 | Various constructions |

---

## 04 - Essential Multiparty Computation

**Total Papers**: 15+ papers
**Time Estimate**: 4-6 weeks
**Priority**: ⭐⭐ Important for distributed systems

### Core MPC Papers

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| A Fair and Efficient Solution to Socialist Millionaires (2001) | ⭐⭐⭐ | 🟡 | **Classic MPC** problem |
| Multiparty Computation with Faulty Majority (1990) - Beaver, Goldwasser | ⭐⭐⭐ | 🔴 | **Foundational** MPC |
| Distributed Key Generation (2010) - Kate | ⭐⭐⭐ | 🟡 | DKG protocols |

### Secret Sharing

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| A Secret Sharing Scheme Based on Group Presentations (2012) | ⭐⭐ | 🔴 | Novel construction |
| Asynchronous Verifiable Secret Sharing (2002) | ⭐⭐⭐ | 🔴 | **Byzantine-robust** VSS |
| Scalable Mechanisms for Rational Secret Sharing (2012) | ⭐⭐ | 🔴 | Game-theoretic approach |

### Password-Authenticated Key Exchange

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| Practical UC Two-Server Password-Auth (2012) - Camenisch et al. | ⭐⭐ | 🔴 | Universally composable PAKE |
| Credential Authenticated Identification (2010) - Camenisch et al. | ⭐⭐ | 🔴 | Advanced authentication |

### Oblivious Transfer

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| 10+ papers in `oblivious transfer/` folder | ⭐⭐⭐ | 🟡-🔴 | **Essential** MPC primitive |

---

## 05 - Essential FHE and Lattices

**Total Papers**: 35+ papers
**Time Estimate**: 6-10 weeks
**Priority**: ⭐⭐⭐ Post-quantum and FHE

### Foundational FHE

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| Fully Homomorphic Encryption [Gentry's thesis] | ⭐⭐⭐ | ⚫ | **THE** FHE breakthrough |
| Towards Constructing FHE without Ciphertext Noise (2008) | ⭐⭐ | ⚫ | Early FHE attempts |

### Lattice-Based Cryptography

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| Lattices [mathematical definitions] (2002) - Brouwer | ⭐⭐⭐ | 🟡 | **Foundation** for lattices |
| 22 papers in `lattice-based cryptography/` folder | ⭐⭐⭐ | 🔴-⚫ | Comprehensive coverage |
| Fast Cryptographic Primitives from Hard Learning Problems (2009) | ⭐⭐⭐ | 🔴 | **LWE-based** crypto |
| Hierarchical IBE Lossy Trapdoor Functions (2012) | ⭐⭐ | 🔴 | Advanced constructions |

### NTRU

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| 8 papers in `lattice-based cryptography/ntru/` | ⭐⭐⭐ | 🟡-🔴 | **NIST finalist** |

### Multilinear Maps

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| Candidate Multilinear Maps from Ideal Lattices (2013) - Garg, Gentry, Halevi | ⭐⭐⭐ | ⚫ | **GGH construction** |
| Practical Multilinear Map over Integers (2013) | ⭐⭐ | ⚫ | CLT construction |

### Circular Security

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| New Definitions and Separations for Circular Security (2012) | ⭐⭐ | 🔴 | Advanced FHE topic |

### Code Obfuscation

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| Obfuscating Circuits via Composite-Order Graded Encoding (2015) | ⭐⭐ | ⚫ | IO constructions |

---

## 06 - Important Applications

**Total Papers**: 50+ papers
**Time Estimate**: Variable (4-8 weeks)
**Priority**: ⭐⭐ Real-world applications

### Cryptocurrencies - Zerocash

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| Zerocash: Decentralized Anonymous Payments (2014) | ⭐⭐⭐ | 🔴 | **Must read** - zkSNARKs in production |
| Zerocash [extended] (2014) | ⭐⭐⭐ | ⚫ | Full technical details |
| Zerocoin (2013) - Miers et al. | ⭐⭐ | 🟡 | Precursor to Zerocash |

### Cryptocurrencies - Privacy Coins

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| CryptoNote v2.0 [Monero] (2013) - Saberhagen | ⭐⭐⭐ | 🟡 | **Monero foundation** |
| ShadowCash (2014) | ⭐⭐ | 🟡 | Ring signatures |

### Cryptocurrencies - General

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| Coda: Decentralized Cryptocurrency at Scale (2018) | ⭐⭐⭐ | 🔴 | **Recursive SNARKs** (now Mina) |
| Hashcash (2002) - Back | ⭐⭐ | 🟢 | **Proof-of-work** origin |

### Blockchain Infrastructure

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| Enabling Blockchain Innovations with Pegged Sidechains (2014) | ⭐⭐ | 🟡 | Sidechain construction |

### E-Cash

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| An Efficient Offline E-Cash (1993) - Brands | ⭐⭐⭐ | 🟡 | **Foundational** e-cash |
| Balancing Accountability and Privacy (2006) - Camenisch et al. | ⭐⭐⭐ | 🔴 | Modern e-cash |
| Compact E-Cash (2007) - Camenisch et al. | ⭐⭐⭐ | 🔴 | Efficient construction |
| Endorsed E-Cash (2007) - Camenisch et al. | ⭐⭐ | 🔴 | Advanced features |
| Untraceable Offline Cash with Observers (1994) - Brands | ⭐⭐ | 🟡 | Observer-based e-cash |
| Distance-Bounding Protocols (1994) - Brands, Chaum | ⭐⭐ | 🟡 | Physical proximity proofs |

### Anonymous Credentials

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| Cryptographic Framework for Controlled Release (2006) | ⭐⭐⭐ | 🔴 | **Important** credentials |
| Computing on Authenticated Data (2011) - Camenisch et al. | ⭐⭐ | 🔴 | Advanced functionality |
| Privacy-Enhanced Access Control (2009) - PRIME Project | ⭐⭐ | 🟡 | Practical system |
| 20+ more papers in `anonymous credentials/` folder | ⭐⭐ | 🟡-🔴 | Comprehensive coverage |

### Messaging Protocols

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| How Secure is TextSecure? (2014) | ⭐⭐ | 🟡 | Signal predecessor analysis |
| Forward Secure Messaging (2015) - Green, Miers | ⭐⭐ | 🔴 | Forward secrecy |
| Ratcheted Encryption and Key Exchange (2016) | ⭐⭐⭐ | 🔴 | **Double Ratchet** theory |
| Perfect Forward Secrecy and Deniability (2011) | ⭐⭐ | 🔴 | OTR-like protocols |
| Datagram TLS (2004) | ⭐⭐ | 🟡 | DTLS foundation |
| Cryptocat (2012) - Kobeissi | ⭐ | 🟢 | Censorship circumvention |

### Oblivious RAM

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| Onion ORAM (2015) | ⭐⭐ | 🔴 | Constant bandwidth ORAM |

### Encrypted Search

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| Deterministic and Efficiently Searchable Encryption (2007) | ⭐⭐ | 🔴 | Searchable encryption |
| Encryption Secure Against Selective Opening (2008) | ⭐⭐ | 🔴 | Advanced security notion |
| Insecurity Against Selective-Opening Attacks (2012) | ⭐ | 🔴 | Security analysis |

### File Systems

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| Tahoe: Least-Authority Filesystem (2008) | ⭐⭐ | 🟡 | Decentralized storage |

### Authenticated Encryption

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| 10+ papers in `authenticated encryption/` folder | ⭐⭐ | 🟡-🔴 | Various constructions |

---

## 07 - Advanced Topics

**Total Papers**: 40+ papers
**Time Estimate**: Variable
**Priority**: ⭐ Specialized topics

### Security Analysis & Critique

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| A Riddle Wrapped in an Enigma (2015) - Koblitz, Menezes | ⭐⭐ | 🟡 | **Provable security** critique |
| Another Look at "Provable Security" (2004) - Koblitz, Menezes | ⭐⭐ | 🟡 | Important perspective |
| The Brave New World of Bodacious Assumptions (2010) | ⭐⭐ | 🟡 | Security assumptions critique |
| The Uneasy Relationship Between Math and Crypto (2007) - Koblitz | ⭐ | 🟢 | Philosophical discussion |
| The Moral Character of Cryptographic Work (2015) - Rogaway | ⭐⭐ | 🟢 | **Ethics** in crypto |
| Another Look at HMQV (2007) - Menezes | ⭐ | 🔴 | Protocol analysis |

### Cryptanalysis

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| Cryptanalysis of Iterated Block Ciphers [thesis] (1997) - Rijmen | ⭐⭐ | 🔴 | By AES co-designer |
| Cryptanalysis of Twofish (2000) | ⭐ | 🔴 | Block cipher analysis |
| On The Design and Security of RC2 (1998) | ⭐ | 🔴 | Historical interest |
| Practical Attack on AES-128 (2012) - Rijmen | ⭐⭐ | 🔴 | Related-key attacks |
| Bleichenbacher's Attack Strikes Again (2014) | ⭐⭐ | 🟡 | **Padding oracle** |
| Format Oracles on OpenPGP (2015) | ⭐ | 🟡 | Practical attacks |

### NSA/GCHQ Documents

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| Black Budget Cryptanalysis (2013) - GCHQ | ⭐ | 🟡 | Historical interest |
| Classification Guide for Cryptanalysis (2005) - NSA | ⭐ | 🟢 | Taxonomy |
| Cryptographic Modernization Guide (2010) - NSA | ⭐ | 🟢 | Standards evolution |
| Crypt Discovery (2011) - NSA, GCHQ | ⭐ | 🟡 | Tools documentation |
| CryptOps Datastore User Guide - GCHQ | ⭐ | 🟡 | Internal tools |
| Internet Anonymity (2011) - NSA | ⭐ | 🟢 | Threat modeling |

### Implementation Guides

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| NaCl: Security Impact of New Crypto Library (2012) - Bernstein et al. | ⭐⭐⭐ | 🟡 | **Must read** for implementers |
| Charm: Framework for Prototyping (2013) - Green | ⭐⭐ | 🟡 | Rapid prototyping |
| Scalable Multiplier Architecture for Finite Fields (2000) | ⭐ | 🔴 | Hardware implementation |

### Blockchain Consensus

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| Keeping Authorities Honest - Decentralized Witness Cosigning (2015) | ⭐⭐ | 🟡 | DECO protocol |

### Random Number Generation

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| Gaussian Random Number Generators (2007) | ⭐ | 🔴 | Specialized topic |

### Time-Lock Puzzles

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| Time-lock Puzzles and Timed-Release Crypto (1996) - Rivest et al. | ⭐⭐ | 🟡 | Interesting construction |

### Honey Encryption

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| Honey Encryption: Beyond Brute-Force (2014) - Juels | ⭐⭐ | 🟡 | Novel security notion |

### OpenPGP

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| OpenPGP-based Financial Instruments (2008) | ⭐ | 🟡 | Novel application |

### Key Management

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| Efficient Group Key Management (2012) | ⭐ | 🔴 | Specialized protocols |

### Post-Quantum Cryptography

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| 21 papers in `post-quantum cryptography/` folder | ⭐⭐⭐ | 🔴-⚫ | **Future-critical** |

### Formal Verification

| Paper | Priority | Difficulty | Notes |
|-------|----------|-----------|-------|
| Papers in `formal verification/` folder | ⭐⭐ | 🔴 | Proving protocol correctness |

---

## 08 - Skip / Not Relevant

**Total Papers**: ~15 papers
**Priority**: ⭐ Can skip for ZK learning
**Note**: Moved here for completeness, but not essential for zero-knowledge focus

### Topics Included:

- Visual cryptography
- Steganography
- Disk encryption formats (LUKS)
- Pure mathematics (syzygies, monster group, quaternions)
- Complexity theory lectures
- Chaotic encryption

**When to read**: Only if specific interest in these topics

---

## Recently Added Papers (From Root Directory)

### Total Moved: 132 papers → Organized into 01-08 folders

**Key Highlights**:

1. **Textbooks** - Now in 01_Math and 02_Crypto
2. **Groth-Sahai Proofs** - Critical addition to 03_ZK
3. **E-Cash Collection** - Complete Camenisch collection in 06_Applications
4. **Cryptocurrency Papers** - Zerocash, Monero, Coda properly organized
5. **Modern Security Analysis** - Koblitz-Menezes critiques in 07_Advanced
6. **Implementation Guides** - NaCl, Charm now easily findable

---

## Papers to Download (2018-2025)

**These papers are NOT in the library but are ESSENTIAL for modern ZK**

### Must Download - zkSNARKs Evolution

| Paper | Year | Priority | Where to Get |
|-------|------|----------|--------------|
| Groth16: On the Size of Pairing-based NIAs | 2016 | ⭐⭐⭐ | https://eprint.iacr.org/2016/260 |
| Bulletproofs | 2017 | ⭐⭐⭐ | https://eprint.iacr.org/2017/1066 |
| STARKs: Scalable Transparent Arguments | 2018 | ⭐⭐⭐ | https://eprint.iacr.org/2018/046 |
| Sonic | 2019 | ⭐⭐ | https://eprint.iacr.org/2019/099 |
| PLONK | 2019 | ⭐⭐⭐ | https://eprint.iacr.org/2019/953 |
| Halo | 2019 | ⭐⭐⭐ | https://eprint.iacr.org/2019/1021 |
| Marlin | 2019 | ⭐⭐ | https://eprint.iacr.org/2019/1047 |
| Fractal | 2019 | ⭐⭐ | https://eprint.iacr.org/2019/1076 |
| SuperSonic | 2019 | ⭐⭐ | https://eprint.iacr.org/2019/1229 |
| Nova | 2021 | ⭐⭐⭐ | https://eprint.iacr.org/2021/370 |
| HyperPlonk | 2022 | ⭐⭐ | https://eprint.iacr.org/2022/1355 |
| Lasso/Jolt | 2023 | ⭐⭐ | https://eprint.iacr.org/2023/1216 |
| Protostar | 2023 | ⭐⭐ | https://eprint.iacr.org/2023/620 |
| ProtoGalaxy | 2023 | ⭐⭐ | https://eprint.iacr.org/2023/1106 |

### Download Command

```bash
# Example: Download Bulletproofs
curl https://eprint.iacr.org/2017/1066.pdf -o "Bulletproofs.pdf"

# Move to appropriate folder
mv Bulletproofs.pdf "03_ESSENTIAL_Zero_Knowledge/range proofs/"
```

### Where to Add Each Paper

- **Groth16, PLONK, Halo** → `03_ESSENTIAL_Zero_Knowledge/zkSNARKs/`
- **Bulletproofs** → `03_ESSENTIAL_Zero_Knowledge/range proofs/`
- **STARKs, Nova** → Create `03_ESSENTIAL_Zero_Knowledge/modern_systems/`
- **Sonic, Marlin, Fractal** → `03_ESSENTIAL_Zero_Knowledge/zkSNARKs/`
- **HyperPlonk, Protostar, ProtoGalaxy** → Advanced folder or modern_systems

---

## Reading Strategies

### For Complete Beginners (0 → Competent)

**Timeline**: 6-12 months

1. **Months 1-2**: 01_Math_Foundations (focus on ⭐⭐⭐ only)
2. **Months 3-4**: 02_Crypto_Primitives (focus on ECC, pairings, hashes)
3. **Months 5-8**: 03_Zero_Knowledge (follow README learning path)
4. **Months 9-10**: 06_Applications (Zerocash, e-cash)
5. **Months 11-12**: Download and read modern papers (2018-2025)

### For Experienced Cryptographers (Competent → Expert)

**Timeline**: 3-6 months

1. **Month 1**: Skim 01-02, deep dive 03_Zero_Knowledge
2. **Month 2**: 04_MPC or 05_FHE (based on interest)
3. **Month 3**: 06_Applications + modern papers
4. **Months 4-6**: Implement systems, contribute to projects

### For Researchers (Expert → Cutting Edge)

**Timeline**: Ongoing

1. Read all ⭐⭐⭐ and ⭐⭐ papers
2. Download ALL modern papers (2018-2025)
3. Follow IACR ePrint for new submissions
4. Attend CRYPTO, EUROCRYPT, ASIACRYPT
5. Join research communities

---

## Study Tips

### Effective Reading

✅ **DO**:
- Read papers multiple times
- Implement key concepts
- Discuss in study groups
- Take detailed notes
- Work through proofs by hand

❌ **DON'T**:
- Skim papers superficially
- Skip mathematical details
- Read out of order (respect prerequisites)
- Ignore papers marked ⭐⭐⭐
- Study in isolation

### Tools for Paper Management

- **Zotero**: Organize PDFs with tags
- **Notion/Obsidian**: Link papers conceptually
- **Anki**: Spaced repetition for key concepts
- **LaTeX**: Take mathematical notes

---

## Summary Statistics

### Total Papers by Folder

| Folder | Papers | Avg. Time | Priority |
|--------|--------|-----------|----------|
| 01 - Math | ~40 | 4-8 weeks | 🔄 Prerequisite |
| 02 - Crypto | ~100 | 6-10 weeks | 🔄 Prerequisite |
| 03 - Zero-Knowledge | ~35 | 8-16 weeks | ⭐⭐⭐ Essential |
| 04 - MPC | ~15 | 4-6 weeks | ⭐⭐ Important |
| 05 - FHE/Lattices | ~35 | 6-10 weeks | ⭐⭐⭐ Essential |
| 06 - Applications | ~50 | 4-8 weeks | ⭐⭐ Important |
| 07 - Advanced | ~40 | Variable | ⭐ Optional |
| 08 - Skip | ~15 | N/A | ⭐ Skip |

**Grand Total**: ~330 organized papers + 100s in legacy folders

### Papers by Priority

- ⭐⭐⭐ **MUST READ**: ~80 papers (core curriculum)
- ⭐⭐ **RECOMMENDED**: ~120 papers (depth)
- ⭐ **OPTIONAL**: ~130 papers (specialization)

### Papers by Difficulty

- 🟢 **Beginner**: ~50 papers
- 🟡 **Intermediate**: ~150 papers
- 🔴 **Advanced**: ~100 papers
- ⚫ **Expert**: ~30 papers

---

## Quick Reference Guides

### "I want to learn X" - Start Here

| Goal | Start With | Then Read | Time |
|------|------------|-----------|------|
| **zkSNARKs** | 01, 02 foundations | 03_ZK → Groth16, PLONK papers | 6-9 months |
| **STARKs** | 01, 02 foundations | 03_ZK basics → Download STARK papers | 6-9 months |
| **Cryptocurrency Privacy** | 01, 02 foundations | 03_ZK → 06_Applications/zerocash | 6-12 months |
| **FHE** | 01_Math (lattices) | 05_FHE → Gentry thesis | 8-12 months |
| **MPC** | 01, 02 foundations | 04_MPC → Garbled circuits | 4-6 months |
| **Post-Quantum Crypto** | 01_Math (lattices) | 05_Lattices → 07_PQC | 6-10 months |
| **Implementation** | Basic crypto knowledge | 00_IMPLEMENTATION_GUIDE | Ongoing |

---

## Maintenance & Updates

**This index should be updated when**:

- New papers are added to the library
- Modern papers (2025+) are downloaded
- Folder structure changes
- Priority ratings need adjustment
- Community feedback suggests changes

**Maintained by**: Library users (community-driven)

---

## Contributing

**Found an error?** Please update this index!

**Added new papers?** Add them to the appropriate section!

**Disagree with priority ratings?** Open a discussion!

---

*This master index is a living document. As zero-knowledge proof systems evolve and new research emerges, this index should be updated to reflect the current state of the field.*

**Last Updated**: 2025-01-01
**Next Review**: 2025-06-01
**Version**: 1.0

---

**Happy Learning! 🚀**

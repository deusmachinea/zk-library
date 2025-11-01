# START HERE - Welcome to ZK-Library!

## What is this library?

This is a curated collection of academic papers to help you learn:
- **Zero-Knowledge Proofs (ZK)** - Prove statements without revealing information
- **Fully Homomorphic Encryption (FHE)** - Compute on encrypted data
- **Multi-Party Computation (MPC)** - Secure collaborative computation
- **Cryptography Foundations** - The mathematics and primitives underlying all cryptographic systems

## Goal

After working through this library, you should be able to:
1. **Understand** how zero-knowledge proofs work
2. **Write** ZK circuits and proofs
3. **Prove** correctness of cryptographic protocols
4. **Implement** secure cryptographic systems

## How to Use This Library

### Step 1: Read the Main Guide
Start with the **[GUIDE.md](../GUIDE.md)** in the root folder - it provides:
- Complete analysis of all folders
- What's essential vs. what to skip
- Recommended reading order
- Time estimates

### Step 2: Follow the Learning Path

The folders are numbered in recommended order:

1. **01_ESSENTIAL_Math_Foundations/** (2-4 weeks)
   - Number theory, algebra, finite fields
   - Handbook of Applied Cryptography
   - Start here if you're new to cryptography

2. **02_ESSENTIAL_Crypto_Primitives/** (4-6 weeks)
   - Elliptic curves, pairings, hashes
   - Signature schemes, commitments
   - Foundation for modern ZK systems

3. **03_ESSENTIAL_Zero_Knowledge/** (8-12 weeks)
   - **YOUR MAIN DESTINATION**
   - All ZK papers including SNARKs, STARKs
   - Most important folder in this library

4. **04_ESSENTIAL_MPC/** (if focusing on MPC)
   - Secret sharing, oblivious transfer
   - Multi-party computation protocols

5. **05_ESSENTIAL_FHE_and_Lattices/** (if focusing on FHE)
   - Lattice-based cryptography
   - Gentry's FHE thesis
   - Post-quantum foundations

6. **06_IMPORTANT_Applications/** (after foundations)
   - Cryptocurrencies (Zerocash, Monero)
   - Anonymous credentials
   - Real-world ZK applications

7. **07_ADVANCED_Topics/** (later)
   - Post-quantum cryptography
   - Specialized encryption schemes
   - Standards and formal verification

8. **08_SKIP_Not_Relevant/** (skip for now)
   - Side channels, visual crypto, etc.
   - Not needed for ZK/FHE/MPC fundamentals

### Step 3: Quick Start (Absolute Beginner)

If you're completely new:

**Week 1-2**: Read basic number theory papers in folder 01
**Week 3-4**: Read "Zero-Knowledge Proofs" lecture by Miller in folder 03
**Week 5-8**: Study Sigma protocols and Schnorr identification
**Week 9-12**: Dive into zkSNARKs

See [GUIDE.md](../GUIDE.md) for detailed week-by-week plan.

## Prerequisites

### Mathematical Background Needed:
- Basic algebra (high school level)
- Some familiarity with modular arithmetic (can be learned here)
- Comfort with mathematical notation
- Willingness to work through proofs

### Programming (Optional but Helpful):
- Python or JavaScript for implementing concepts
- Helps solidify understanding

## Tips for Success

1. **Don't skip the math** - Everything builds on number theory and algebra
2. **Work through examples** - Don't just read, do the problems
3. **Implement concepts** - Code helps understanding
4. **Take notes** - Summarize each paper in your own words
5. **Be patient** - This material is challenging but rewarding
6. **Join communities** - Find ZK Discord servers, forums, study groups

## Recommended External Resources

While this library is comprehensive, you may also benefit from:

### Online Courses:
- Dan Boneh's Cryptography I & II (Coursera)
- zkSNARKs MOOC
- MIT OpenCourseWare: Introduction to Cryptography

### Books (not in this repo):
- "Introduction to Modern Cryptography" - Katz & Lindell
- "Handbook of Applied Cryptography" (included here)

### Practical Tutorials:
- Circom/SnarkJS tutorials for hands-on ZK
- ZK-learning.org resources
- 0xPARC learning group materials

### For Security Enclaves:
- Intel SGX documentation (separate topic)
- ARM TrustZone guides
- Note: Enclaves are hardware-based, different from cryptographic ZK

## Folder Structure Summary

```
00_START_HERE/           ← You are here!
01_ESSENTIAL_Math_Foundations/     ⭐⭐⭐ Start here
02_ESSENTIAL_Crypto_Primitives/    ⭐⭐⭐ Then this
03_ESSENTIAL_Zero_Knowledge/       ⭐⭐⭐ YOUR MAIN GOAL
04_ESSENTIAL_MPC/                  ⭐⭐⭐ For MPC focus
05_ESSENTIAL_FHE_and_Lattices/     ⭐⭐⭐ For FHE focus
06_IMPORTANT_Applications/         ⭐⭐  After foundations
07_ADVANCED_Topics/                ⭐   Much later
08_SKIP_Not_Relevant/              ❌   Skip for now
```

## Time Estimates

- **Foundations only** (ZK basics): 3-6 months
- **ZK mastery** (can write proofs): 6-12 months
- **ZK + MPC**: 8-15 months
- **ZK + FHE**: 9-18 months
- **All topics**: 12-24 months

These assume 10-20 hours per week of focused study.

## Questions?

1. Check [GUIDE.md](../GUIDE.md) for detailed folder analysis
2. Look at README files in each numbered folder
3. Join online ZK communities for help

## Ready to Begin?

**Next step**: Go to [01_ESSENTIAL_Math_Foundations/README.md](../01_ESSENTIAL_Math_Foundations/README.md)

Good luck on your journey into zero-knowledge cryptography!

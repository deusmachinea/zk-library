# 08 - SKIP: Not Relevant for ZK/FHE/MPC Beginners

## ❌ Skip This Folder (For Now)

This folder contains topics that are **NOT essential** for learning zero-knowledge proofs, FHE, or MPC.

## Why These Topics Are Skipped

If your goal is to:
- ✅ Understand and write zero-knowledge proofs
- ✅ Learn FHE (Fully Homomorphic Encryption)
- ✅ Study MPC (Multi-Party Computation)
- ✅ Master cryptographic foundations

**Then skip this folder entirely.**

These topics are either:
1. **Too specialized**: Niche research areas not relevant to mainstream crypto
2. **Implementation-focused**: About secure coding, not cryptographic theory
3. **Tangential**: Interesting but not on the critical path

## What's in This Folder

### Folders You Can Skip:

1. **side channels/** (26 papers)
   - **What it is**: Physical attacks on crypto implementations
   - Timing attacks, power analysis, cache attacks
   - **Why skip**: Implementation security, not cryptographic foundations
   - **When to read**: Only when implementing real-world systems
   - **Example**: "Timing Attacks on Implementations of Diffie-Hellman"

2. **visual cryptography/** (2 papers)
   - **What it is**: Sharing secret images visually
   - **Why skip**: Niche topic, completely unrelated to ZK/FHE/MPC
   - **When to read**: Never (unless specifically interested)

3. **knot theory/** (4 papers)
   - **What it is**: Using mathematical knots for cryptography
   - **Why skip**: Experimental, not mainstream cryptography
   - **When to read**: Advanced research only

4. **quaternions/** (3 papers)
   - **What it is**: 4D number system for crypto
   - **Why skip**: Very specialized, not used in ZK/FHE/MPC
   - **When to read**: If interested in exotic crypto math

5. **hyperelliptic/** (6 papers)
   - **What it is**: Alternative to elliptic curves
   - **Why skip**: Elliptic curves are standard; hyperelliptic are niche
   - **When to read**: Advanced research, curve specialists only

6. **camellia/** (1 paper)
   - **What it is**: Specific block cipher
   - **Why skip**: Just one cipher, not fundamental
   - **When to read**: If implementing Camellia specifically

7. **differential cryptanalysis/** (2 papers)
   - **What it is**: Technique to break block ciphers
   - **Why skip**: Cryptanalysis, not building ZK systems
   - **When to read**: If designing new ciphers

8. **otr/** (7 papers)
   - **What it is**: Off-the-Record messaging protocol
   - **Why skip**: Specific application, not fundamental crypto
   - **When to read**: If building secure messaging apps

9. **patents/** (1 paper)
   - **What it is**: Patent documents
   - **Why skip**: Legal, not technical learning material
   - **When to read**: Never for learning

10. **quantum cryptography/** (8 papers)
    - **What it is**: Quantum key distribution, quantum protocols
    - **Why skip**: Different paradigm (physics-based, not math-based)
    - **When to read**: Only if specifically interested in quantum crypto
    - **Note**: This is NOT post-quantum cryptography (which IS relevant)

11. **quantum algorithms & cryptanalysis/** (2 papers)
    - **What it is**: Quantum algorithms (Shor's, Grover's)
    - **Why skip**: Unless you're studying quantum computing specifically
    - **When to read**: For understanding quantum threat to classical crypto

12. **isogeny-based cryptography/** (1 paper)
    - **What it is**: Post-quantum crypto using isogenies
    - **Why skip**: Advanced post-quantum topic, recently broken (SIKE)
    - **When to read**: Advanced post-quantum research

13. **supersingular isogeny/** (4 papers)
    - **What it is**: Specific isogeny constructions
    - **Why skip**: See above (isogeny-based)
    - **When to read**: Advanced research only

14. **rank-based cryptography/** (1 paper)
    - **What it is**: Experimental post-quantum approach
    - **Why skip**: Not mainstream, experimental
    - **When to read**: Advanced post-quantum research

## Side Channels: Special Note

**Side channels** (26 papers) is the largest folder here.

**What are side channels?**
- Physical information leakage from crypto implementations
- Timing (how long operations take)
- Power consumption (how much energy used)
- Electromagnetic emanations
- Cache behavior

**Examples**:
- Measuring time to factor a number reveals information
- Power analysis can extract keys from smart cards
- Cache timing can leak AES keys

**Why skip for now?**
- You're learning cryptographic theory, not implementation
- Side channels are about secure coding and hardware
- Not needed to understand ZK/FHE/MPC concepts

**When to read?**
- When implementing cryptography in production
- When working with hardware (smart cards, embedded systems)
- After you master the theory

**Important**: Side channels are real threats! But learn the theory first, then secure implementation.

## What You Should Focus On Instead

Instead of this folder, spend time on:

1. **01_ESSENTIAL_Math_Foundations/** ⭐⭐⭐
   - Number theory, algebra, finite fields

2. **02_ESSENTIAL_Crypto_Primitives/** ⭐⭐⭐
   - Elliptic curves, pairings, hashes

3. **03_ESSENTIAL_Zero_Knowledge/** ⭐⭐⭐
   - Your main goal!

4. **04_ESSENTIAL_MPC/** ⭐⭐⭐ (if interested)
   - Secret sharing, oblivious transfer

5. **05_ESSENTIAL_FHE_and_Lattices/** ⭐⭐⭐ (if interested)
   - Lattices, LWE, Gentry's FHE

6. **06_IMPORTANT_Applications/** ⭐⭐
   - Real-world ZK applications

## If You're Curious About These Topics

### Side Channels:
- **Book**: "The Hardware Hacking Handbook" - Jasper van Woudenberg
- **Course**: Hardware Security courses (separate from crypto theory)
- **When**: After you've implemented crypto systems

### Visual Cryptography:
- Interesting visual demos, but not useful for ZK/FHE/MPC
- Fun for presentations, not essential

### Knot Theory Crypto:
- Mostly experimental
- Not used in practice
- Pure research interest

### Quaternions:
- 4D extension of complex numbers
- Some niche crypto uses
- Not mainstream

### Quantum Cryptography (QKD):
- Physics-based key distribution
- Different from math-based crypto
- Requires quantum hardware
- Not scalable yet
- Separate field from ZK/FHE/MPC

### Post-Quantum vs. Quantum Cryptography:
- **Quantum Cryptography (QKD)**: Uses quantum mechanics, here in SKIP folder
- **Post-Quantum Cryptography**: Math-based crypto resistant to quantum computers, in ADVANCED or FHE folders
- Don't confuse the two!

## Exception: When These Might Be Relevant

### Side Channels → Relevant if:
- You're implementing ZK proofs in production
- Working on hardware wallets
- Building secure systems (smart cards, etc.)

### Quantum Algorithms → Relevant if:
- You want to understand why lattices are post-quantum secure
- Studying Shor's algorithm (breaks RSA/ECDLP)
- Understanding quantum threat

### Differential Cryptanalysis → Relevant if:
- Designing new block ciphers
- Analyzing cipher security
- Deep dive into symmetric crypto

## Summary Table

| Folder | Relevance to ZK/FHE/MPC | When to Read |
|--------|-------------------------|--------------|
| side channels | ❌ Implementation | When coding production systems |
| visual cryptography | ❌ Irrelevant | Never (unless curious) |
| knot theory | ❌ Experimental | Never (pure research) |
| quaternions | ❌ Niche | Never (unless interested) |
| hyperelliptic | ❌ Niche curves | Advanced curve research |
| camellia | ❌ Specific cipher | If using Camellia |
| differential cryptanalysis | ❌ Cryptanalysis | If designing ciphers |
| otr | ❌ Specific protocol | If building messaging |
| patents | ❌ Legal docs | Never |
| quantum cryptography (QKD) | ❌ Different field | If interested in QKD |
| quantum algorithms | ⚠️ Marginal | To understand quantum threat |
| isogeny-based crypto | ❌ Advanced PQC | Advanced research |
| supersingular isogeny | ❌ Advanced PQC | Advanced research |
| rank-based crypto | ❌ Experimental | Advanced research |

## FAQs

**Q: Should I read side channel papers?**
A: Not for learning crypto theory. Read them when implementing systems.

**Q: Is quantum cryptography the same as post-quantum cryptography?**
A: No! Quantum crypto uses quantum mechanics (QKD). Post-quantum crypto is math-based but quantum-resistant (lattices, etc.).

**Q: Are these topics useless?**
A: No, just not relevant for ZK/FHE/MPC learning. They have their own use cases.

**Q: When should I come back to this folder?**
A: After mastering folders 01-05. Or when you have specific need (e.g., side channels for implementation).

**Q: Is hyperelliptic crypto important?**
A: Not really. Elliptic curves are standard. Hyperelliptic is academic.

**Q: What about visual cryptography?**
A: Fun demo, not practical. Skip unless you want cool visual effects.

## Final Advice

**Don't let curiosity distract you from the main path.**

Learning ZK/FHE/MPC takes 6-12+ months of focused study. These topics will only distract you.

**Stay focused**:
1. Math foundations (01)
2. Crypto primitives (02)
3. Zero-knowledge (03)
4. MPC or FHE (04-05)
5. Applications (06)

**Then**, if you have time and interest, explore advanced topics (07) or come back here.

---

## You Shouldn't Be Reading This

If you're a beginner following the learning path, **close this folder** and go back to:

→ [00_START_HERE/README.md](../00_START_HERE/README.md)

**Focus on what matters. Skip the rest.**

---

**Remember**: Time is limited. Spend it on essential topics (folders 01-05), not tangential ones.

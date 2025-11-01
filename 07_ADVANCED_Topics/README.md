# 07 - ADVANCED Topics

## Priority: ⭐ ADVANCED (Read Much Later)

## Purpose

This folder contains topics that are:
- Advanced extensions of core concepts
- Specialized applications
- Important but not essential for beginners
- Best learned after mastering folders 01-05

## Time Estimate

**Varies by topic** - Pick based on interest

## Prerequisites

Before this folder:
- ✅ **01-03 ESSENTIAL folders** - Must have solid foundations
- ⚠️ **04-05 ESSENTIAL folders** - Helpful depending on topic
- ⚠️ **06 Applications** - Good to see practical uses first

**Don't rush here!** These are advanced topics requiring strong foundations.

## What's in This Folder

### Folders (in recommended reading order):

1. **post-quantum cryptography/** (21 papers)
   - Lattice-based schemes (overlaps with 05)
   - Hash-based signatures
   - Code-based crypto
   - Post-quantum ZK

2. **security models/** (1 paper)
   - Formal security definitions
   - Provable security frameworks

3. **private information retrieval/** (3 papers)
   - Query databases without revealing query
   - Related to MPC

4. **formal verification/** (1 paper)
   - Proving crypto protocols correct
   - Machine-checked proofs

5. **block ciphers/** (4 papers)
   - AES, Twofish, etc.
   - Symmetric encryption foundations

6. **stream ciphers/** (3 papers)
   - ChaCha20, Salsa20
   - Symmetric crypto

7. **random number generators/** (5 papers)
   - Cryptographically secure RNGs
   - Important for implementations

8. **rsa/** (6 papers)
   - Classical public-key crypto
   - Historical importance

9. **elgamal/** (2 papers)
   - Classical public-key encryption
   - Based on discrete log

10. **ibe/** (Identity-Based Encryption) (5 papers)
    - Advanced public-key crypto
    - Uses pairings

11. **attribute-based encryption/** (1 paper)
    - Very advanced access control

12. **standards/** (4 papers)
    - Cryptographic standards
    - When implementing real systems

## Learning Path by Interest

### Interest 1: Post-Quantum Cryptography

**If you're concerned about quantum computers breaking crypto:**

**Read** (from post-quantum cryptography/):
1. ⭐⭐⭐ Overview papers on post-quantum crypto
2. ⭐⭐⭐ NIST PQC competition papers
3. ⭐⭐ Lattice-based schemes (also in folder 05)
4. ⭐⭐ Hash-based signatures (SPHINCS+)
5. ⭐ Code-based crypto (McEliece)

**Key Concepts**:
- Quantum threat to RSA/ECDLP (Shor's algorithm)
- Quantum-resistant assumptions:
  - Lattices (LWE, Ring-LWE)
  - Hash functions
  - Codes
  - Multivariate polynomials
- NIST standards: Kyber (encryption), Dilithium (signatures)

**Why This Matters**:
- Prepare for post-quantum world
- Lattice crypto (folder 05) is post-quantum
- Future-proofing systems

**Note**: Much overlap with **05_ESSENTIAL_FHE_and_Lattices/** since lattices are post-quantum.

### Interest 2: Classical Crypto (RSA, ElGamal, etc.)

**If you want historical context or need these for legacy systems:**

**Read**:
1. ⭐⭐ RSA papers (rsa/)
2. ⭐⭐ ElGamal papers (elgamal/)
3. ⭐⭐ Diffie-Hellman (if available)

**Key Concepts**:
- RSA: Factoring-based encryption and signatures
- ElGamal: Discrete log-based encryption
- Diffie-Hellman: Key exchange

**Why Read**:
- Historical importance
- Understand evolution to modern crypto
- Many systems still use RSA

**Why Not Essential**:
- Modern ZK uses elliptic curves (folder 02), not RSA
- Quantum computers will break RSA/DH
- Important but not on critical path for ZK

### Interest 3: Symmetric Crypto

**If you need to understand ciphers, hashes, RNGs:**

**Read**:
1. ⭐⭐ Block cipher papers (block ciphers/)
   - AES design and analysis
   - Other ciphers (Twofish, etc.)
2. ⭐ Stream cipher papers (stream ciphers/)
   - ChaCha20, Salsa20
3. ⭐⭐ Random number generator papers (random number generators/)
   - CSPRNGs
   - Important for implementations

**Key Concepts**:
- Block ciphers: AES, modes of operation
- Stream ciphers: Keystream generation
- RNGs: Entropy, pseudorandomness

**Why Read**:
- Understanding symmetric crypto helps
- RNGs crucial for implementations
- Good background knowledge

**Why Not Essential**:
- ZK focuses on public-key and number-theoretic crypto
- Hashes (folder 02) are more relevant than ciphers

### Interest 4: Advanced Public-Key Crypto

**If you want to explore beyond basics:**

**Read**:
1. ⭐⭐ IBE papers (ibe/)
   - Identity-Based Encryption
   - Uses pairings (folder 02)
2. ⭐ Attribute-Based Encryption (attribute-based encryption/)
   - Very advanced access control
   - Also uses pairings

**Key Concepts**:
- IBE: Encrypt to identity (email address) not public key
- ABE: Access policies in ciphertext
- Both use pairing-based crypto

**Why Read**:
- Shows advanced pairing applications
- Elegant crypto constructions

**Why Not Essential**:
- Not directly used in ZK/MPC/FHE
- Advanced applications

### Interest 5: Security & Verification

**If you want to prove protocols correct:**

**Read**:
1. ⭐⭐ Security models papers (security models/)
   - Formal definitions
   - Provable security
2. ⭐ Formal verification papers (formal verification/)
   - Machine-checked proofs
   - EasyCrypt, CryptoVerif

**Key Concepts**:
- Game-based security proofs
- Reduction-based security
- Formal methods for crypto

**Why Read**:
- Understand how security is proven
- Important for research
- Building verified systems

**Why Not Essential**:
- Can use crypto without proving it
- Advanced research topic

### Interest 6: Private Information Retrieval

**If interested in querying privately:**

**Read** (from private information retrieval/):
1. ⭐⭐ PIR introduction papers
2. ⭐ Computational PIR vs. Information-theoretic PIR

**Key Concepts**:
- Query database without revealing query
- Related to MPC and OT
- Applications: private search

**Why Read**:
- Interesting MPC-related problem
- Real-world applications (privacy-preserving search)

**Why Not Essential**:
- Specialized topic
- Not core to ZK/FHE

## Paper Reading Priority

### Post-Quantum (Highest Priority in This Folder):

1. ⭐⭐⭐ NIST PQC overview
2. ⭐⭐⭐ Kyber/Dilithium papers
3. ⭐⭐ Hash-based signatures
4. ⭐⭐ Lattice schemes (also in folder 05)

### Security & Foundations:

5. ⭐⭐ Security models papers
6. ⭐ Formal verification

### Classical Crypto (Historical Context):

7. ⭐⭐ RSA papers
8. ⭐ ElGamal papers

### Symmetric Crypto:

9. ⭐⭐ RNG papers (important for implementations)
10. ⭐ Block cipher papers (if interested)
11. ⭐ Stream cipher papers (if interested)

### Advanced Public-Key:

12. ⭐ IBE papers
13. ⭐ ABE papers
14. ⭐ PIR papers

### Implementation:

15. ⭐ Standards papers (when building real systems)

## When to Read This Folder

### Post-Quantum:
- After folder 05 (lattices)
- When concerned about quantum threat
- When implementing post-quantum systems

### Classical Crypto (RSA, ElGamal):
- For historical understanding
- When maintaining legacy systems
- After modern crypto (folders 01-03)

### Symmetric Crypto:
- When implementing systems (RNGs)
- For general crypto knowledge
- Not urgent for ZK learning

### Advanced Public-Key (IBE, ABE):
- After mastering pairings (folder 02)
- When exploring advanced constructions
- Research interest

### Security Models:
- When doing crypto research
- To understand proofs in papers
- Advanced academic interest

### PIR:
- After MPC (folder 04)
- When building private search
- Specialized interest

## Common Pitfalls

❌ **Don't**:
- Read this folder before folders 01-05
- Think RSA is relevant for modern ZK (it's not)
- Skip post-quantum if you learned lattices (they're related)
- Read everything (pick topics based on interest)

✅ **Do**:
- Focus on post-quantum if interested in future crypto
- Read RNG papers if implementing crypto
- Understand security models if doing research
- Be selective - these are advanced topics

## Connection to Core Topics

### How This Folder Relates to ZK/FHE/MPC:

**Post-Quantum** ↔ **FHE (Folder 05)**:
- Both use lattices
- Lattice-based crypto is post-quantum
- Overlap in techniques

**Security Models** ↔ **All Crypto**:
- How to prove crypto secure
- Applies to ZK, MPC, FHE

**PIR** ↔ **MPC (Folder 04)**:
- Related problem
- Uses OT and MPC techniques

**IBE/ABE** ↔ **Pairings (Folder 02)**:
- Uses pairing-based crypto
- Advanced applications

**RSA/ElGamal** ↔ **Historical**:
- Foundation of public-key crypto
- Understand evolution to modern systems

**RNGs** ↔ **Implementations**:
- Needed for all crypto implementations
- Practical importance

## Self-Assessment

After selectively reading from this folder, you should be able to:

✅ (Post-Quantum) Understand quantum threat and lattice-based solutions
✅ (Classical) Explain RSA and ElGamal (historical context)
✅ (Symmetric) Understand block ciphers and RNGs basics
✅ (Advanced) Know about IBE and ABE concepts
✅ (Security) Understand how crypto security is proven
✅ (PIR) Grasp private information retrieval problem

**Note**: You don't need to master all topics, just those relevant to your goals.

## Next Steps

### After This Folder:

**For cutting-edge research**:
- Read recent papers (2020+)
- Follow IACR ePrint
- Join research communities

**For implementation**:
- Study standards (NIST, FIPS)
- Learn crypto engineering
- Read side channel papers (folder 08, when needed)

**For specialization**:
- Deep dive into chosen area (ZK, MPC, FHE, or PQC)
- Contribute to open-source projects
- Join research groups

## Additional Resources

### Post-Quantum:
- NIST PQC website
- PQShield blog
- Cloudflare crypto blog (PQC articles)

### Classical Crypto:
- "Twenty Years of Attacks on RSA" - Boneh
- Cryptography textbooks (Katz-Lindell, etc.)

### Security:
- Provable Security courses
- EasyCrypt/CryptoVerif documentation

### Standards:
- NIST publications
- IETF RFCs

## FAQ

**Q: Should I read this folder?**
A: Selectively, based on interest. Not all topics are necessary.

**Q: Is post-quantum crypto important?**
A: Yes! Quantum computers are coming. Lattice crypto (folder 05) is already post-quantum.

**Q: Do I need to know RSA for ZK?**
A: Not really. Modern ZK uses elliptic curves, not RSA. But RSA is good historical context.

**Q: What about standards?**
A: Read when implementing real systems. Not needed for learning theory.

**Q: Should I learn IBE/ABE?**
A: Only if interested in advanced pairing-based crypto. Not essential for ZK.

**Q: Are RNGs important?**
A: Yes, for implementations. Every crypto system needs good randomness.

## Summary

This folder is a **choose your own adventure**:

- **Must read**: Post-quantum (if interested in future crypto)
- **Good to know**: Security models, RNGs
- **Optional**: Classical crypto (RSA, ElGamal) for history
- **Specialized**: IBE, ABE, PIR (only if specifically interested)
- **When needed**: Standards, formal verification

**Don't try to read everything.** Pick topics relevant to your goals.

---

**Remember**: You've reached the advanced stage. Be selective and focus on what matters for your goals. You don't need to know everything—just what's relevant to your work.

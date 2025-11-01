# Conference Papers Index (2005-2025)

This index organizes conference papers from the `crypto_conferences/` directory by topic and relevance to the ZK learning path. Papers are mapped to the corresponding tutorial folders (01-08) for easier navigation.

## How to Use This Index

- **Must Read**: Essential papers for understanding core concepts
- **Recommended**: Important papers that deepen understanding
- **Optional**: Advanced or specialized topics
- **Reference**: For specific use cases or research

---

## Zero-Knowledge Proofs (→ 03_ESSENTIAL_Zero_Knowledge/)

### Foundational ZK Papers

**2005:**
- `Undonditional Characterstics of Non-Interactive Zero-Knowledge.pdf` - **Must Read** - Foundational NIZK theory

**2006:**
- `Non-interactive Zaps and New Techniques for NIZK.pdf` - **Must Read** - Important NIZK construction techniques
- `On Signatures of Knowledge.pdf` - **Recommended** - Connects signatures to ZK proofs

**2007:**
- `Zero-Knowledge from Secure Multiparty Computation.pdf` - **Recommended** - Connecting ZK and MPC

### Modern ZK Systems (zkSNARKs, STARKs, PLONK)

**Key Papers to Find in 2018-2025 Conferences:**

Look for these topics in recent years:
- **STARKs**: Scalable Transparent Arguments of Knowledge
- **PLONK**: Permutations over Lagrange-bases for Oecumenical Noninteractive arguments of Knowledge
- **Halo 2**: Recursive proof composition without trusted setup
- **Nova**: Recursive SNARKs
- **Bulletproofs**: Short proofs for arithmetic circuits
- **Groth16**: Efficient zkSNARK construction
- **Marlin**: Universal and updatable zkSNARKs

**Search Strategy:**
```bash
# Find STARK papers
find crypto_conferences/ -name "*STARK*" -o -name "*stark*"

# Find PLONK papers
find crypto_conferences/ -name "*PLONK*" -o -name "*plonk*"

# Find Bulletproofs
find crypto_conferences/ -name "*Bulletproof*"

# Find recursive proofs
find crypto_conferences/ -name "*recursive*" -o -name "*Halo*" -o -name "*Nova*"
```

---

## Fully Homomorphic Encryption (→ 05_ESSENTIAL_FHE_and_Lattices/)

**2008:**
- `towards constructing Fully Homomorphic Encryption without Ciphertext Noise from Group Theorstructing_Fully_Homomorphic_Encryption_.pdf` - **Recommended** - Early FHE construction attempts

**Recent Years (2018-2025):**
Look for:
- TFHE (Torus FHE)
- CKKS scheme
- Bootstrapping optimizations
- FHE applications

---

## Multiparty Computation (→ 04_ESSENTIAL_MPC/)

**Topics to search for in conferences:**
- Garbled circuits optimizations
- MPC protocols
- Threshold cryptography
- Secure two-party computation

---

## Lattice-Based Cryptography (→ 05_ESSENTIAL_FHE_and_Lattices/)

**Topics to search for:**
- Learning With Errors (LWE)
- Ring-LWE
- NTRU variants
- Lattice-based signatures (Dilithium, Falcon)
- Post-quantum cryptography

---

## Pairing-Based Cryptography (→ 02_ESSENTIAL_Crypto_Primitives/)

**Topics to search for:**
- Bilinear pairings
- BLS signatures
- Identity-based encryption
- Attribute-based encryption

---

## Applications (→ 06_IMPORTANT_Applications/)

### Cryptocurrencies and Blockchain

**Topics to search for:**
- Zero-knowledge rollups (zk-rollups)
- Privacy coins
- Blockchain scaling
- Smart contract privacy
- Consensus mechanisms

### Anonymous Credentials

**Topics to search for:**
- Anonymous credential systems
- Attribute-based credentials
- Privacy-preserving authentication

---

## How to Extract Relevant Papers

### Step 1: Identify Your Topic

Determine which area you're studying:
1. Math foundations
2. Crypto primitives
3. Zero-knowledge
4. MPC
5. FHE/Lattices
6. Applications
7. Advanced topics

### Step 2: Search Conference Papers

Use grep or find to search by keyword:

```bash
# Example: Find all ZK-related papers
find crypto_conferences/ -name "*.pdf" | grep -i "zero-knowledge\|zkSNARK\|zk-SNARK\|NIZK"

# Example: Find all STARK papers
find crypto_conferences/ -name "*.pdf" | grep -i "STARK"

# Example: Find all FHE papers
find crypto_conferences/ -name "*.pdf" | grep -i "homomorphic\|FHE"

# Example: Find all MPC papers
find crypto_conferences/ -name "*.pdf" | grep -i "multiparty\|MPC"

# Example: Find all lattice papers
find crypto_conferences/ -name "*.pdf" | grep -i "lattice\|LWE\|NTRU"
```

### Step 3: Copy to Appropriate Folder

Once you identify a relevant paper:

```bash
# Example: Copy a STARK paper to ZK folder
cp "crypto_conferences/2023/STARK_paper.pdf" "03_ESSENTIAL_Zero_Knowledge/modern_systems/"

# Example: Copy an FHE paper
cp "crypto_conferences/2020/TFHE_paper.pdf" "05_ESSENTIAL_FHE_and_Lattices/fhe/"
```

---

## Priority Papers by Year (2018-2025)

### 2018-2019: Modern ZK Systems Emergence

**Priority Topics:**
- Bulletproofs introduction
- STARK papers (Ben-Sasson et al.)
- Sonic/PLONK early work

### 2020-2021: Scaling and Optimization

**Priority Topics:**
- PLONK improvements
- Halo introduction
- ZK-rollup designs
- FHE optimizations (TFHE, CKKS improvements)

### 2022-2023: Recursive Proofs and Production Systems

**Priority Topics:**
- Nova (recursive SNARKs)
- Halo 2 improvements
- Production zkEVM papers
- Practical FHE applications

### 2024-2025: Latest Developments

**Priority Topics:**
- Latest proving system optimizations
- Hardware acceleration
- New cryptographic assumptions
- Real-world deployment case studies

---

## Recommended Conference Sources

The `crypto_conferences/` directory likely contains papers from:

- **CRYPTO**: Top-tier, highly theoretical
- **EUROCRYPT**: Top-tier, European focus
- **ASIACRYPT**: Top-tier, Asian focus
- **TCC**: Theory of Cryptography Conference
- **PKC**: Public Key Cryptography
- **CCS**: ACM Conference on Computer and Communications Security
- **USENIX Security**: Systems and applied crypto
- **S&P (Oakland)**: Security and privacy
- **NDSS**: Network and Distributed System Security

---

## Quick Reference: What to Look For

### For Beginners (01-03 folders)
- Introductory ZK papers (2005-2010)
- Tutorial-style papers
- Survey papers on zkSNARKs

### For Intermediate Learners (04-05 folders)
- MPC protocol papers
- FHE construction papers
- Lattice-based crypto fundamentals

### For Advanced Learners (06-07 folders)
- Latest proving systems (2020-2025)
- Implementation papers
- Security analysis papers
- Novel applications

---

## Creating Your Custom Learning Path

1. **Start with GUIDE.md** - Follow the week-by-week plan
2. **Supplement with conference papers** - Use this index to find relevant recent papers
3. **Focus on your goals**:
   - Researcher: Read theory papers from CRYPTO/EUROCRYPT
   - Developer: Read implementation papers from USENIX/CCS
   - Application builder: Read zkEVM, zk-rollup papers

---

## Tools for Paper Discovery

### Command-Line Search Examples

```bash
# Find all papers with "SNARK" in the name
find crypto_conferences/ -iname "*snark*"

# Find papers from 2022-2025 only
find crypto_conferences/202[2-5]/ -name "*.pdf"

# Count papers by year
for year in {2005..2025}; do
  count=$(find crypto_conferences/$year/ -name "*.pdf" 2>/dev/null | wc -l)
  echo "$year: $count papers"
done

# Search PDF contents for keywords (if pdfgrep is installed)
pdfgrep -i "zero knowledge" crypto_conferences/**/*.pdf
```

---

## Contributing to This Index

As you explore the conference papers:

1. Note which papers are essential for your learning path
2. Add them to the appropriate numbered folders (01-08)
3. Update the README in that folder
4. Share your findings by updating this index

---

## Next Steps

1. **Explore Recent Papers**: Focus on 2018-2025 for latest ZK developments
2. **Create Themed Collections**: Group papers by specific topics (STARKs, PLONK, etc.)
3. **Update Folder READMEs**: Add conference paper references to existing topic folders
4. **Build Implementation Guide**: Link papers to practical coding resources

---

*Last Updated: 2025*
*Total Conference Years Covered: 2005-2025 (21 years)*
*Estimated Total Papers: 100+ across all conferences*

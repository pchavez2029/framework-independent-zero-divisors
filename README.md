# The Canonical Six

Framework-independent zero divisor patterns in higher-dimensional Cayley-Dickson algebras with Lean 4 formal verification.

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.17402495.svg)](https://doi.org/10.5281/zenodo.17402495)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Paper: CC BY 4.0](https://img.shields.io/badge/Paper-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

## Paper

**Title:** Framework-Independent Zero Divisor Patterns in Higher-Dimensional Cayley-Dickson Algebras: Discovery and Verification of The Canonical Six

**Author:** Paul Chavez (Chavez AI Labs)

**Published:** Zenodo - [DOI: 10.5281/zenodo.17402495](https://doi.org/10.5281/zenodo.17402495) (all versions)

**Latest Version:** v1.2 (January 2026) - [Direct link](https://zenodo.org/records/18357723)

## Abstract

We report the discovery of 12 zero divisor patterns in 16-dimensional sedenion space exhibiting dimensional persistence and framework-dependent behavior, with six patterns demonstrating framework independence across both Cayley-Dickson and Clifford algebraic constructions. Computational verification across five Cayley-Dickson dimensions (16D through 256D) and two Clifford algebra dimensions (16D and 32D) demonstrates exact preservation of zero divisor properties through successive dimensional doublings, achieving machine precision (≈ 10⁻¹⁵) in all successful tests.

The patterns divide equally: six universal structures (The Canonical Six) maintain zero divisor properties in both associative (Clifford) and non-associative (Cayley-Dickson) frameworks, while six construction-dependent patterns succeed only in Cayley-Dickson algebras, revealing a fundamental 50/50 split. Representing only 3.6% of all 168 sedenion zero divisors, these framework-independent patterns exhibit superlinear dimensional stability—maintaining exact structure through 256-fold complexity increase—suggesting they occupy mathematically distinguished positions indicative of deeper organizational principles in higher-dimensional algebras.

**Partial formal verification in Lean 4 (822 lines, 83% coverage) provides machine-verified mathematical proofs of core structural claims.**

## Key Findings

- **12 patterns** with dimensional persistence (16D → 256D)
- **6 universal patterns** (The Canonical Six) work identically in both Cayley-Dickson and Clifford algebras
- **50/50 split** between framework-independent and construction-dependent patterns
- **3.6% universality ratio** - only 6 of 168 sedenion zero divisors show framework independence
- **Machine precision** verification (≈ 10⁻¹⁵) across 7 dimensions
- **83% formal verification** in Lean 4 (10 of 12 patterns proven)

## The Canonical Six (Universal Patterns)

Framework-independent zero divisor patterns that maintain exact structure through:

| Pattern | Formula | Frameworks |
|---------|---------|------------|
| 18 | (e₁ + e₁₄) × (e₃ + e₁₂) = 0 | CD ✓ Clifford ✓ |
| 59 | (e₃ + e₁₂) × (e₅ + e₁₀) = 0 | CD ✓ Clifford ✓ |
| 84 | (e₄ + e₁₁) × (e₆ + e₉) = 0 | CD ✓ Clifford ✓ |
| 102 | (e₁ − e₁₄) × (e₃ − e₁₂) = 0 | CD ✓ Clifford ✓ |
| 104 | (e₁ − e₁₄) × (e₅ + e₁₀) = 0 | CD ✓ Clifford ✓ |
| 124 | (e₂ − e₁₃) × (e₆ + e₉) = 0 | CD ✓ Clifford ✓ |

These patterns persist through:
- Both associative (Clifford) and non-associative (Cayley-Dickson) frameworks
- Five dimensional doublings: 16D → 32D → 64D → 128D → 256D
- 256-fold complexity increase with perfect structural preservation

## Formal Verification

**New in v1.2:** Partial formal verification in Lean 4 confirms the mathematical validity of these patterns beyond computational approximation.

**Verification Coverage:**
- 10 of 12 patterns formally proven in CD4 (sedenions)
- Dimensional persistence verified through CD6 (256D)
- Framework independence mathematically verified (not just observed)
- 822 lines of machine-checked Lean 4 code

See: [`lean-formalization/`](lean-formalization/) directory for complete formalization files and technical details.

## Repository Contents

### Papers
- **`canonical_six_v1_2.pdf`** - Latest version (v1.2) with formal verification ⭐
- `canonical_six_v1.1.pdf` - Version 1.1 with AI acknowledgements
- `Hyperwormholes_Paper.pdf` - Original version 1.0

### Formal Verification
- **`lean-formalization/`** - Lean 4 formal proofs (NEW in v1.2)
  - `dc08bbac-primary.lean` - Primary formalization (822 lines, 83% coverage)
  - `c038a2e4-alternative.lean` - Alternative approach (283 lines)
  - `LEAN_README.md` - Technical documentation

### Source
- `main.tex` - LaTeX source

## Version History

### Version 1.2 (January 2026) - DOI: [10.5281/zenodo.18357723](https://zenodo.org/records/18357723)
**Major Update:**
- Added Section 8: Formal Verification in Lean 4
- Includes 822 lines of machine-verified proofs (83% coverage)
- Supplementary Lean formalization files
- Updated abstract to reference formal verification
- **Latest version - use this for citations**

### Version 1.1 (November 2025) - DOI: [10.5281/zenodo.17574868](https://zenodo.org/records/17574868)
- Added acknowledgements for AI assistance (Claude, Gemini)
- Updated with transparent research methodology disclosure

### Version 1.0 (October 2025) - DOI: [10.5281/zenodo.17402496](https://zenodo.org/records/17402496)
- Original publication
- Discovery and computational verification

## Citation

**Cite the latest version (v1.2 with formal verification):**

```bibtex
@article{chavez2026canonical,
  title={Framework-Independent Zero Divisor Patterns in Higher-Dimensional
         Cayley-Dickson Algebras: Discovery and Verification of The Canonical Six},
  author={Chavez, Paul},
  year={2026},
  month={January},
  doi={10.5281/zenodo.18357723},
  url={https://zenodo.org/records/18357723},
  note={Version 1.2 with Lean 4 formal verification}
}
```

**For concept DOI (always resolves to latest):**

```bibtex
@article{chavez2025canonical,
  title={Framework-Independent Zero Divisor Patterns in Higher-Dimensional
         Cayley-Dickson Algebras: Discovery and Verification of The Canonical Six},
  author={Chavez, Paul},
  year={2025},
  doi={10.5281/zenodo.17402495},
  url={https://doi.org/10.5281/zenodo.17402495},
  note={Concept DOI - always resolves to latest version}
}
```

## Significance

This discovery challenges the characterization of sedenions and higher Cayley-Dickson algebras as "pathological." The existence of framework-independent patterns with demonstrable superlinear stability suggests exploitable mathematical structure rather than arbitrary complexity. Like imaginary numbers, non-Euclidean geometries, and Hawking radiation before them, these patterns may represent the next instance of a recurring historical pattern: what initially appears pathological often contains fundamental structure awaiting theoretical understanding.

## Publication Status

- **Latest version (v1.2):** https://zenodo.org/records/18357723
- **All versions:** https://doi.org/10.5281/zenodo.17402495


## Contact

**Paul Chavez**
Founder, Chavez AI Labs
Independent Researcher, Computational Mathematics
Los Angeles, California

Email: iknowpi@gmail.com


## License

- **Paper and documentation:** [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)
- **Code:** [MIT License](https://opensource.org/licenses/MIT)

## Acknowledgments

This research was conducted with substantial assistance from AI systems (Claude, Gemini, Claude Code). All mathematical claims were computationally verified to machine precision. See paper for detailed methodology and acknowledgments.

---

*"Better math, less suffering"* - Chavez AI Labs

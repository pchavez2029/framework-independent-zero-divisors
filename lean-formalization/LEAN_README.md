# Lean 4 Formal Verification Files

Partial formal verification of zero divisor patterns using Harmonic Math's Aristotle proof assistant.

## Files

### dc08bbac-primary.lean (Primary - Recommended)
- **Status:** 83% complete (10 of 12 patterns verified)
- **Foundation:** Rational-based (ℚ) Cayley-Dickson construction
- **Verified Theorems:**
  - Patterns 18, 19, 58, 59, 81, 84, 101, 102, 104, 124 in CD4 sedenions
  - Dimensional persistence: Patterns 18, 59, 84 in CD5 (pathions) and CD6 (chingons)
  - Framework independence: Universal patterns verified in Clifford Cl(5,0)
  - CD-specific patterns verified to fail in Clifford Cl(4,0)
- **Lines:** 822
- **Use this file if:** Building upon or extending verification

### c038a2e4-alternative.lean
- **Status:** Partial (foundational properties only)
- **Foundation:** Real-based (ℝ) Cayley-Dickson construction
- **Verified Theorems:** CD1, CD2 foundational properties
- **Lines:** 283
- **Use this file if:** Prefer ℝ-based approach or need alternative proof strategies

## Verification Scope

**Currently Verified:**
- ✓ 10 of 12 discovered patterns in CD4 sedenions
- ✓ Dimensional persistence through CD6 (256D)
- ✓ Framework independence (Clifford vs Cayley-Dickson)
- ✓ 50/50 universal/construction-dependent classification

**Not Yet Verified:**
- Pattern 103: (e₁ - e₁₄) × (e₄ + e₁₁) = 0 (expansion defined, proof incomplete)
- Pattern 121: (e₂ - e₁₃) × (e₁ - e₁₄) = 0 (expansion defined, proof incomplete)

## Technical Details

- **Lean Version:** leanprover/lean4:v4.24.0
- **Mathlib Version:** f897ebcf72cd16f89ab4577d0c826cd14afaafc7
- **Verification Method:** Computational (`decide +kernel`)
- **Precision:** Machine precision (~10⁻¹⁵)

## Building on These Files

The primary file (dc08bbac-primary.lean) provides solid foundations for:
1. Completing proofs for patterns 103, 121
2. Extending dimensional persistence to additional patterns
3. Additional Clifford framework comparisons

The existing infrastructure (Cayley-Dickson construction, basis definitions, multiplication rules) is production-ready.

## Citation

Generated using Harmonic Math's Aristotle proof assistant (https://harmonic.fun/)

Research and verification direction: Paul Chavez, Chavez AI Labs

## Paper Reference

For complete mathematical context, see:
"Framework-Independent Zero Divisor Patterns in Higher-Dimensional Cayley-Dickson Algebras: 
Discovery and Verification of The Canonical Six"
DOI: https://doi.org/10.5281/zenodo.17402495
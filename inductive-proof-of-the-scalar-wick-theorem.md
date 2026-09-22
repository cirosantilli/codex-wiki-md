# Inductive proof of the scalar Wick theorem

↑ **Parent:** [Wick's theorem](wick-s-theorem.md)

Split each free [real scalar field](real-scalar-field.md) as $\phi=\phi^{(-)}+\phi^{(+)}$, into creation and annihilation parts. For chronologically ordered arguments, the first field has the latest time. Multiplying it into a [normal-ordered product](normal-ordered-product.md) of the remaining fields gives

$$
\phi_1:\!\prod_{r\in I}\phi_r\!:
=:\!\phi_1\prod_{r\in I}\phi_r\!:
+\sum_{j\in I}[\phi_1^{(+)},\phi_j^{(-)}]:\!\prod_{r\in I\setminus\{j\}}\phi_r\!:.
$$

This follows by commuting the annihilation part through each creation part; each [commutator](commutator.md) is a scalar, and all creation parts commute among themselves, as do all annihilation parts. The scalar commutator is the [Feynman propagator](feynman-propagator.md) for the chronological pair. Induction on the number of fields therefore lists every partial pairing exactly once: either field 1 remains unpaired or it pairs with one $j$. This proves the [Wick theorem](wick-s-theorem.md) for free bosonic fields, including the empty pairing. Vacuum expectation retains only complete pairings. The identities are understood for regulated or smeared [operator-valued distributions](operator-valued-distribution.md).

## ↑ Ancestors (6)

1. [Wick's theorem](wick-s-theorem.md)
2. [Perturbative quantum field theory](perturbative-quantum-field-theory-split.md)
3. [Quantum field theory](quantum-field-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-42/1/solution.md)

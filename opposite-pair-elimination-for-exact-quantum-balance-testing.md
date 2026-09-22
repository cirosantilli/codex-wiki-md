# Opposite-pair elimination for exact quantum balance testing

↑ **Parent:** [Deutsch-Jozsa algorithm](deutsch-jozsa-algorithm.md)

For an even-length Boolean string, one phase query followed by a known [unitary extension](unitary-extension-of-a-finite-dimensional-isometry.md) can produce a zero-pair outcome with amplitude proportional to the zero-minus-one imbalance, or an index pair with amplitude proportional to the difference of their phase signs. A zero-pair observation certifies nonbalance. Every nonzero pair has opposite bits, so deleting it preserves the imbalance and allows recursion on two fewer indices. Ending with an empty list certifies balance. This [quantum circuit](quantum-circuit-split.md) is exact on all inputs and uses at most half the original length in queries, even without the constant-or-balanced promise.

## ↑ Ancestors (5)

1. [Deutsch-Jozsa algorithm](deutsch-jozsa-algorithm.md)
2. [Quantum theory](quantum-theory-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-58/3/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-58/3/b/iii/solution.md)

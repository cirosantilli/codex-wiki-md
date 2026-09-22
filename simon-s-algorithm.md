<h1 id="simon-s-algorithm">Simon's algorithm</h1>

↑ **Parent:** [Simon's problem](simon-s-problem.md)

Simon's algorithm prepares hidden-subgroup [coset states](coset-state.md), applies the [quantum Fourier transform](quantum-fourier-transform-split.md) over $(\mathbb Z_2)^n$, and samples vectors $y$ satisfying $y\cdot p=0$ over $\mathbb F_2$. Repeated samples and [Gaussian elimination](gaussian-elimination.md) recover $p$ with $O(n)$ oracle queries and polynomial computation.

To solve [Simon's problem](simon-s-problem.md), prepare a [uniform quantum superposition](uniform-quantum-superposition.md), evaluate the function coherently into a second [quantum register](quantum-register.md), and perform [Simon Fourier sampling](simon-fourier-sampling.md) on the first. Each run produces a uniform [binary string](binary-string.md) $z$ with $z\cdot s=0$ over the two-element [field](field.md). Once the observed rows have [matrix rank](matrix-rank.md) $n-1$, [Gaussian elimination](gaussian-elimination.md) recovers $s$ as the unique nonzero element of their [kernel](kernel-of-a-linear-map-split.md). The [random spanning of a binary vector space](random-spanning-of-a-binary-vector-space.md) bounds the required number of runs.

**Table of contents**

- [Simon Fourier sampling](simon-fourier-sampling.md)
- [Simon coset state](simon-coset-state.md)
- [Expected query count for Simon sampling](expected-query-count-for-simon-sampling.md)
- [Single-sample distribution in Simon's algorithm](single-sample-distribution-in-simon-s-algorithm.md)
- [Orthogonal complement over the binary field](orthogonal-complement-over-the-binary-field.md)

## ↑ Ancestors (7)

1. [Simon's problem](simon-s-problem.md)
2. [Hidden subgroup problem](hidden-subgroup-problem.md)
3. [Quantum Fourier transform](quantum-fourier-transform-split.md)
4. [Quantum theory](quantum-theory-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Classical collision query bound for Simon's problem](classical-collision-query-bound-for-simon-s-problem.md)
- [Expected query count for Simon sampling](expected-query-count-for-simon-sampling.md)
- [Solution](past-exam-of-the-introduction-to-quantum-information-course-of-the-university-of-oxford/2015/1/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3/15c/b/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-324/4/b/iii/solution.md)
- [Quantum oracle](quantum-oracle.md)
- [Random spanning of a binary vector space](random-spanning-of-a-binary-vector-space.md)
- [Simon coset state](simon-coset-state.md)

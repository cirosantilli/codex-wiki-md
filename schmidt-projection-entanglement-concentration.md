# Schmidt projection entanglement concentration

↑ **Parent:** [Entanglement concentration](entanglement-concentration.md)

For $n$ copies of a normalized [pure state](pure-state.md) $\alpha|00\rangle+\beta|11\rangle$, regroup Alice's and Bob's tensor factors. Alice performs a [projective measurement](projective-measurement.md) of the total number $k$ of zeroes, preserving all coherence among strings with that count. The outcome has [binomial distribution](binomial-distribution.md)

$$
p_k=\binom nk|\alpha|^{2k}|\beta|^{2(n-k)}.
$$

Each retained string has the same complex amplitude $\alpha^k\beta^{n-k}$, so, up to a common phase, the conditional [quantum state](quantum-state.md) is

$$
|T_k\rangle=\binom nk^{-1/2}\sum_{z(x)=k}|x\rangle_A|x\rangle_B.
$$

Its equal [Schmidt coefficients](schmidt-coefficient.md) make it a [maximally entangled state](maximally-entangled-state.md) of [Schmidt rank](schmidt-rank.md) $\binom nk$. Alice sends the count to Bob. They can relabel the corresponding local [computational basis](computational-basis.md) strings with local unitary operations, and convert the resulting resource to [Bell pairs](bell-pair.md). Measuring the individual bits instead would reveal the entire string and leave a [product state](product-state.md).

**Table of contents**

- [Tripartite Schmidt projection entanglement concentration](tripartite-schmidt-projection-entanglement-concentration.md)

## ↑ Ancestors (8)

1. [Entanglement concentration](entanglement-concentration.md)
2. [Entangled state](entangled-state.md)
3. [Reduced density matrix](reduced-density-matrix.md)
4. [Bell state](bell-state-split.md)
5. [Quantum theory](quantum-theory-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-53/3/solution.md)

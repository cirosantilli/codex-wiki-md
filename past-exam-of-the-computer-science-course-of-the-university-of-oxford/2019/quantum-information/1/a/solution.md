<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [basic measurement](../../../../../basic-measurement.md) is specified by an [orthonormal basis](../../../../../orthonormal-basis.md) $\{|b_j\rangle\}_{j=0}^{d-1}$, with outcome $j$ associated with the rank-one [orthogonal projection](../../../../../orthogonal-projection.md) $P_j=|b_j\rangle\langle b_j|$. For a normalized [pure state](../../../../../pure-state.md) $|\psi\rangle$, the [Born rule](../../../../../born-rule.md) gives

$$
\boxed{p(j)=\langle\psi|P_j|\psi\rangle=|\langle b_j|\psi\rangle|^2.}
$$

The [probabilities](../../../../../probability.md) sum to one because $\sum_jP_j=I$. Conditional on an outcome with $p(j)>0$, the [post-measurement state](../../../../../post-measurement-state.md) is

$$
\boxed{\frac{P_j|\psi\rangle}{\sqrt{p(j)}}=\frac{\langle b_j|\psi\rangle}{|\langle b_j|\psi\rangle|}|b_j\rangle,}
$$

which represents $|b_j\rangle$ up to a [global phase](../../../../../global-phase.md). An outcome of zero [probability](../../../../../probability.md) has no conditional state to normalize. For a [density matrix](../../../../../density-matrix-split.md) $\rho$, the corresponding expressions are $p(j)=\operatorname{Tr}(P_j\rho)$ and $P_j\rho P_j/p(j)$. If the outcome is ignored, the [nonselective projective measurement](../../../../../nonselective-projective-measurement.md) instead produces $\sum_jP_j\rho P_j$, generally a [mixed state](../../../../../mixed-state.md).[§2.3, Definition 2.34 and the outcome-probability rule; specialize to rank-one orthogonal projections](../../../../../the-theory-of-quantum-information-by-john-watrous/basic-notions-of-quantum-information.md)

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Quantum information](../../../quantum-information-split.md)
4. [2019](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)

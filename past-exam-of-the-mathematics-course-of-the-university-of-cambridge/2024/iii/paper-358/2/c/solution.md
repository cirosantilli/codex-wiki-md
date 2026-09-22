<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Here [functional calculus convergence](../../../../../../functional-calculus-convergence.md) means that for every $f\in C(\mathbb T)$,

$$
\boxed{
\langle f(A_n)P_nv,P_nw\rangle
\longrightarrow
\langle f(A)v,w\rangle
\qquad(v,w\in\mathcal H).}
$$

Embed $\mathcal H_n$ in $\mathcal H$ and write $\widetilde A_n=P_n^*A_nP_n$. The hypothesis gives $\widetilde A_n\rightharpoonup A$ in the [weak operator topology](../../../../../../weak-operator-topology.md). Since $A_n$ and $A$ are [unitary operators](../../../../../../unitary-operator.md),

$$
\|\widetilde A_nv-Av\|^2
=\|P_nv\|^2+\|v\|^2
-2\operatorname{Re}\langle\widetilde A_nv,Av\rangle
\longrightarrow0.
$$

Thus $\widetilde A_n\to A$ in the [strong operator topology](../../../../../../strong-operator-topology.md). Applying the same argument to the adjoints gives $\widetilde A_n^*\to A^*$ strongly.

Products of uniformly bounded strongly convergent operators converge strongly, so for every integer $k$,

$$
P_n^*A_n^kP_n\longrightarrow A^k
$$

strongly, with negative $k$ interpreted through adjoints. Therefore convergence holds for every [Laurent polynomial](../../../../../../laurent-polynomial.md). The [Stone-Weierstrass theorem](../../../../../../stone-weierstrass-theorem.md) says that Laurent polynomials are uniformly dense in $C(\mathbb T)$. Since the continuous functional calculus is contractive, uniform approximation finishes the proof for every $f\in C(\mathbb T)$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 358](../../../paper-358-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

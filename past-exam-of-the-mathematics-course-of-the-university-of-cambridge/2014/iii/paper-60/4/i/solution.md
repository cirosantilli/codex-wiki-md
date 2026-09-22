<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

[Nielsen's pure-state conversion theorem](../../../../../../nielsen-s-pure-state-conversion-theorem.md) gives the exact deterministic [LOCC](../../../../../../local-operations-and-classical-communication.md) criterion. Let the [Schmidt decompositions](../../../../../../schmidt-decomposition.md) be $|\psi\rangle=\sum_j\sqrt{\lambda_j}|a_jb_j\rangle$ and $|\phi\rangle=\sum_j\sqrt{\mu_j}|a'_jb'_j\rangle$. The vectors $\lambda,\mu$ consist of squared [Schmidt coefficients](../../../../../../schmidt-coefficient.md), equivalently the eigenvalues of either reduced [density operator](../../../../../../density-matrix.md). Order each in decreasing order and pad with zeros to a common length $d$.

Then deterministic conversion is possible if and only if

$$
\boxed{\lambda\prec\mu,\quad\text{meaning}\quad
\sum_{j=1}^k\lambda_j\leq\sum_{j=1}^k\mu_j\ (1\leq k<d),\qquad
\sum_{j=1}^d\lambda_j=\sum_{j=1}^d\mu_j=1.}
$$

This is [majorization](../../../../../../majorization.md), with the input vector majorized by the output vector. The direction matters: a maximally entangled state has a uniform vector, which is majorized by a product state's vector $(1,0,\ldots)$, so entanglement can be discarded by [LOCC](../../../../../../local-operations-and-classical-communication.md). The criterion is for certain exact conversion, without catalysts or postselection on a successful branch.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

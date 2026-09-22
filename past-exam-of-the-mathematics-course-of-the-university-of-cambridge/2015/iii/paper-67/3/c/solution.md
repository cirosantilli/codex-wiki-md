<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [local Hamiltonian problem](../../../../../../local-hamiltonian-problem.md) is a [promise problem](../../../../../../promise-problem.md) specified by a sum $H=\sum_{j=1}^M h_j$ on $n$ [qubits](../../../../../../qubit.md), where $M$ is polynomial in $n$, each Hermitian term acts on at most a fixed number $k$ of [qubits](../../../../../../qubit.md), and the terms and two thresholds $a<b$ are described with polynomially many bits. The promise gap satisfies $b-a\geq1/\operatorname{poly}(n)$. In a convenient normalization, $0\leq h_j\leq I$. The task is to distinguish

$$
\boxed{\text{YES: }\lambda_{\min}(H)\leq a,
\qquad
\text{NO: }\lambda_{\min}(H)\geq b.}
$$

There is no required answer when the minimum energy lies between the thresholds. A formulation with Hermitian terms of polynomially bounded norm is equivalent: shift each term by a known scalar lower bound and rescale all terms by a polynomial bound to obtain [positive semidefinite](../../../../../../positive-semidefinite-matrix.md) terms of norm at most one, while shifting and rescaling $a,b$ in parallel. The promise gap remains inverse-polynomial.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

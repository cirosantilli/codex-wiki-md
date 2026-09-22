<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let

$$
H_\pm=\pm J\sum_jh_{j,j+1},
\qquad
h_{j,j+1}=\mathbf S_j\mathbin\cdot\mathbf S_{j+1},
$$

where the two signs describe the [Heisenberg antiferromagnet](../../../../../../heisenberg-antiferromagnet.md) and [Heisenberg ferromagnet](../../../../../../heisenberg-ferromagnet.md). A standard [Lieb-Robinson bound](../../../../../../lieb-robinson-bound.md) is obtained by iterating the [Heisenberg picture](../../../../../../heisenberg-picture.md) equation and bounding nested [commutators](../../../../../../commutator.md) by [operator norms](../../../../../../operator-norm.md). Its constants depend on the interaction only through quantities such as

$$
\sup_x\sum_{X\ni x}|X|\,\|\Phi(X)\|e^{\mu\operatorname{diam}X}.
$$

Changing $J$ to $-J$ changes neither the supports nor the norms $\|\Phi(X)\|$. Every term in the nested-commutator estimate acquires at most an irrelevant sign before its absolute value is taken. Therefore both chains obey exactly the same estimate

$$
\|[A(t),B]\|
\leq C\|A\|\|B\|e^{-\mu(d(A,B)-v_{\rm LR}|t|)}
$$

with the same $C,\mu$, and Lieb-Robinson velocity $v_{\rm LR}$. No unitary equivalence of the two Hamiltonians is required.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 343](../../../paper-343-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

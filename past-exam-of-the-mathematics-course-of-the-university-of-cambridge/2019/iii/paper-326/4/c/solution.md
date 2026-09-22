<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $u^\dagger=u_J^\dagger$, $p^\dagger=A^*\mu^\dagger\in\partial J(u^\dagger)$, and $r_\alpha=Au_\alpha-f$. The [subgradient inequality](../../../../../../subgradient-inequality.md), the [dual pairing](../../../../../../dual-pairing.md) bound, and $Au^\dagger=f$ give

$$
J(u_\alpha)-J(u^\dagger)\geq\langle p^\dagger,u_\alpha-u^\dagger\rangle
=\langle\mu^\dagger,r_\alpha\rangle
\geq-\|\mu^\dagger\|\|r_\alpha\|.
$$

Minimality of $u_\alpha$ in the [exact penalty method](../../../../../../exact-penalty-method.md) gives

$$
\|r_\alpha\|+\alpha[J(u_\alpha)-J(u^\dagger)]\leq0.
$$

Combining them yields

$$
(1-\alpha\|\mu^\dagger\|)\|r_\alpha\|\leq0.
$$

The coefficient is strictly positive, so

$$
\boxed{Au_\alpha=f.}
$$

Now minimality gives $J(u_\alpha)\leq J(u^\dagger)$, and exact feasibility plus the defining minimality of $u^\dagger$ gives the reverse inequality. Thus $u_\alpha$ is a [J-minimizing solution](../../../../../../j-minimizing-solution.md). Finally,

$$
\boxed{D_J^{p^\dagger}(u_\alpha,u^\dagger)
=J(u_\alpha)-J(u^\dagger)-\langle\mu^\dagger,A(u_\alpha-u^\dagger)\rangle=0.}
$$

This [exact-penalty threshold from a source condition](../../../../../../exact-penalty-threshold-from-a-source-condition.md) does not require one-homogeneity; convexity and the source subgradient suffice. If $\mu^\dagger=0$, the same argument works for every $\alpha>0$, interpreting the upper threshold as infinite.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

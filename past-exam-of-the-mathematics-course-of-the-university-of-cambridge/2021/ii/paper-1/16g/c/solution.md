<h1 id="16g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

If some $T_i$ were inconsistent, it would prove every formula by the classical principle of explosion. Because $T_i$ is a [deductively closed set of formulae](../../../../../../deductively-closed-set-of-formulae.md), it would then contain every formula and could have no proper extension. This contradicts $T_i\subsetneq T_{i+1}$. Thus every $T_i$ is consistent.

Let

$$
T=\bigcup_{i=0}^{\infty}T_i.
$$

If $T$ were inconsistent, the [finite character of formal proofs](../../../../../../finite-character-of-formal-proofs.md) would give a finite inconsistent subset $R\subseteq T$. The chain is increasing, so all finitely many members of $R$ lie in some common $T_N$. Then $T_N$ would be inconsistent, a contradiction. Hence $T$ is consistent.

If $T\vdash\varphi$, a proof again uses only finitely many assumptions from $T$, all lying in some $T_N$. Thus

$$
T_N\vdash\varphi.
$$

Since $T_N$ is deductively closed, $\varphi\in T_N\subseteq T$. Therefore $T$ is deductively closed.

Finally, suppose that $T$ were finitary. Part (b) would provide a finite $R\subseteq T$ such that $R\vdash T$. Choose $N$ with $R\subseteq T_N$. Then $T_N\vdash T$; since $T_N$ is deductively closed, this implies $T\subseteq T_N$. But

$$
T_N\subsetneq T_{N+1}\subseteq T,
$$

a contradiction. Consequently $T$ is not finitary, proving the [increasing union of deductively closed sets](../../../../../../increasing-union-of-deductively-closed-sets.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [16G](../../16g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

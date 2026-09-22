<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $X_1,\ldots,X_n$ be IID with full-support mass function $Q$ on a finite alphabet $\mathcal A$, and let the [empirical distribution](../../../../../../type-information-theory.md) be

$$
\widehat P_n(a)=\frac1n\sum_{i=1}^n\mathbf1_{\{X_i=a\}}.
$$

Suppose $E$ is a set of probability mass functions satisfying $E=\overline{E^\circ}$ and that the [information projection](../../../../../../information-projection.md) $P^*$ minimizes $D(P\|Q)$ over $E$. Then the limiting [Sanov theorem](../../../../../../sanov-theorem.md) is

$$
\lim_{n\to\infty}-\frac1n\log_2Q^n(\widehat P_n\in E)
=D(P^*\|Q).
$$

For each $n$-type $P$, the [method of types](../../../../../../method-of-types.md) gives

$$
(n+1)^{-|\mathcal A|}2^{-nD(P\|Q)}
\leq Q^n(T_P)\leq2^{-nD(P\|Q)},
$$

and there are at most $(n+1)^{|\mathcal A|}$ types. Summing the upper bounds over types in $E$ gives the large-deviation upper bound. For the lower bound, choose types $P_n\in E$ converging to an interior distribution arbitrarily close to $P^*$ and use the lower type-class bound. Polynomial factors disappear after applying $-n^{-1}\log_2$, and continuity of divergence finishes the proof.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

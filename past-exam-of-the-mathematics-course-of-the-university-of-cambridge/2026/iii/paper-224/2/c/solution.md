<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let

$$
\mathcal C_\delta=\{R:D(R\Vert P)\leq\delta\},
\qquad
D(\delta)=\min_{R\in\mathcal C_\delta}D(R\Vert Q).
$$

The minimum exists because the probability simplex is compact. Let $R^*$ be the [information projection](../../../../../../information-projection.md) of $Q$ onto the closed [convex set](../../../../../../convex-set.md) $\mathcal C_\delta$. Its Pythagorean inequality says that every $R\in\mathcal C_\delta$ satisfies

$$
D(R\Vert Q)-D(R\Vert R^*)\geq D(R^*\Vert Q)=D(\delta).
$$

For a string $x_1^n$ of [type](../../../../../../type-information-theory.md) $R\in\mathcal C_\delta$, this gives

$$
\frac{Q^{\otimes n}(x_1^n)}{(R^*)^{\otimes n}(x_1^n)}
=2^{-n[D(R\Vert Q)-D(R\Vert R^*)]}
\leq2^{-nD(\delta)}.
$$

Summing over the decision region $B_n$ proves the exact bound

$$
\boxed{e_1^{(n)}=Q^{\otimes n}(B_n)
\leq2^{-nD(\delta)}(R^*)^{\otimes n}(B_n)
\leq2^{-nD(\delta)}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Using [multi-index notation](../../../../../../multi-index-notation.md), the [Schwartz space](../../../../../../schwartz-space.md) is

$$
\mathcal S(\mathbb R^n)=\left\{\varphi\in C^\infty(\mathbb R^n):p_{\alpha,\beta}(\varphi)=\sup_{x\in\mathbb R^n}|x^\alpha\partial^\beta\varphi(x)|<\infty\text{ for all }\alpha,\beta\right\}.
$$

A [sequence](../../../../../../sequence.md) $\varphi_m$ converges to $\varphi$ in this [Fréchet space](../../../../../../frechet-space.md) when $p_{\alpha,\beta}(\varphi_m-\varphi)\to0$ for every $\alpha,\beta$. The space $\mathcal S'(\mathbb R^n)$ of [tempered distributions](../../../../../../tempered-distribution.md) is the [continuous dual](../../../../../../continuous-dual-space-split.md) of $\mathcal S(\mathbb R^n)$, and $u_m\to u$ there means [weak convergence of distributions](../../../../../../weak-convergence-of-distributions.md), namely $\langle u_m,\varphi\rangle\to\langle u,\varphi\rangle$ for every $\varphi\in\mathcal S$.

Continuity of a [linear functional](../../../../../../linear-functional.md) immediately implies that $\varphi_m\to0$ entails $\langle u,\varphi_m\rangle\to0$. Conversely, enumerate the Schwartz [seminorms](../../../../../../seminorm.md) as $p_1,p_2,\ldots$. If $u$ were not continuous, then for each $m$ one could choose $\varphi_m$ such that

$$
p_j(\varphi_m)\leq\frac1m\quad(1\leq j\leq m),
\qquad
|\langle u,\varphi_m\rangle|\geq1.
$$

Every fixed seminorm tends to zero along this sequence, so $\varphi_m\to0$ in $\mathcal S$, contradicting the assumed sequential property. This is the [sequential continuity criterion for a linear map on a metrizable topological vector space](../../../../../../sequential-continuity-criterion-for-a-linear-map-on-a-metrizable-topological-vector-space.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 327](../../../paper-327-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

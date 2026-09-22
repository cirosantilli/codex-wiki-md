<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Freiling theorem](../../../../../../freiling-theorem.md) gives

$$
\boxed{A_{<\omega_1}(\mathbb R)\ \Longleftrightarrow\ \neg\mathrm{CH}}.
$$

First assume the [Continuum hypothesis](../../../../../../continuum-hypothesis.md) and fix a [well-order](../../../../../../well-order.md) $(r_\alpha)_{\alpha<\omega_1}$ of the [real numbers](../../../../../../real-number.md). Define $f(r_\alpha)=\{r_\beta:\beta\leq\alpha\}$. Each value is countable. For any pair, one index is at most the other, so at least one of $x\in f(y)$ or $y\in f(x)$ holds. The same holds for $x=y$, since $x\in f(x)$. This violates the [Freiling axiom of symmetry](../../../../../../freiling-axiom-of-symmetry.md).

Conversely, assume $|\mathbb R|>\aleph_1$ and let $f$ assign a countable set to each real. Choose $X\subseteq\mathbb R$ of [cardinality](../../../../../../cardinality.md) $\aleph_1$. By [infinite cardinal arithmetic](../../../../../../infinite-cardinal-arithmetic.md),

$$
\left|X\cup\bigcup_{x\in X}f(x)\right|\leq\aleph_1<|\mathbb R|.
$$

Choose $y$ outside this union. Since $f(y)$ is countable and $X$ is uncountable, choose $x\in X\setminus f(y)$. Then $y\notin f(x)$ and $x\notin f(y)$, with $x\ne y$. This proves the [Freiling axiom of symmetry](../../../../../../freiling-axiom-of-symmetry.md) and completes both implications.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 121](../../../paper-121-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

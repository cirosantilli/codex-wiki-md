<h1 id="30j/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The stochastic gradients obey

$$
\lVert G_s\rVert_2\leq G:=\frac{M}{\log2}.
$$

The [nonexpansiveness of metric projection](../../../../../../nonexpansiveness-of-metric-projection.md) and the [subgradient inequality](../../../../../../subgradient-inequality.md) imply, after conditioning on $\beta_s$,

$$
2\eta\,\mathbb E[f(\beta_s)-f(\widehat\beta)]
\leq\mathbb E\lVert\beta_s-\widehat\beta\rVert_2^2
-\mathbb E\lVert\beta_{s+1}-\widehat\beta\rVert_2^2
+\eta^2G^2.
$$

Summing telescopes. Since both $\beta_1$ and $\widehat\beta$ lie in the radius-$R$ set $C$, their distance is at most $2R$. By the [Jensen inequality](../../../../../../jensen-s-inequality.md) and convexity of $f$,

$$
\mathbb E f(\bar\beta)-f(\widehat\beta)
\leq\frac{2R^2}{\eta k}+\frac{\eta M^2}{2\{\log2\}^2}.
$$

Choose

$$
\boxed{\eta=\frac{2R\log2}{M\sqrt k}}.
$$

The two terms are then equal, and

$$
\boxed{\mathbb E f(\bar\beta)-f(\widehat\beta)
\leq\frac{2MR}{\log(2)\sqrt k}}.
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [30J](../../30j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

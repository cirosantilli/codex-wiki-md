<h1 id="23f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [layer cake representation](../../../../../../layer-cake-representation.md) with $\varphi(t)=t^p$ gives

$$
\lVert Mf\rVert_p^p
=p\int_0^\infty s^{p-1}
\lambda(\{Mf>s\})\,ds.
$$

For each $s>0$, split

$$
f=f_0+f_1,
\qquad f_0=f\mathbf1_{\{|f|>s/2\}},
\qquad f_1=f\mathbf1_{\{|f|\leq s/2\}}.
$$

Since $Mf_1\leq s/2$ and the maximal operator is sublinear,

$$
\{Mf>s\}\subseteq\{Mf_0>s/2\}.
$$

The weak $(1,1)$ [Hardy-Littlewood maximal inequality](../../../../../../hardy-littlewood-maximal-inequality.md) therefore gives

$$
\lambda(\{Mf>s\})
\leq\frac{2C_1}{s}
\int_{\{|f|>s/2\}}|f(x)|\,dx.
$$

Substitution into the distribution formula and another application of [Tonelli theorem](../../../../../../tonelli-theorem.md) yield

$$
\begin{aligned}
\lVert Mf\rVert_p^p
&\leq2pC_1\int_{\mathbb R^n}|f(x)|
\int_0^{2|f(x)|}s^{p-2}\,ds\,dx\\
&=\frac{2^ppC_1}{p-1}\lVert f\rVert_p^p.
\end{aligned}
$$

Thus the [Strong Lp bound for the Hardy-Littlewood maximal function](../../../../../../strong-lp-bound-for-the-hardy-littlewood-maximal-function.md) holds with

$$
\boxed{\ \lVert Mf\rVert_p\leq
\left(\frac{2^ppC_1}{p-1}\right)^{1/p}\lVert f\rVert_p.\ }
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [23F](../../23f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

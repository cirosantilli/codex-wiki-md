<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose a locally finite cover $(U_\alpha)$ such that on every chart meeting $Y$ there is a smooth defining function $f_\alpha$ with

$$
Y\cap U_\alpha=f_\alpha^{-1}(0),
\qquad df_\alpha|_Y\ne0,
$$

and take $f_\alpha=1$ on charts disjoint from $Y$. On an overlap, the supplied division lemma extends

$$
g_{\alpha\beta}=\frac{f_\alpha}{f_\beta}
$$

smoothly across $Y$. After shrinking the charts, this extension is nowhere zero. The identities $g_{\alpha\beta}g_{\beta\gamma}=g_{\alpha\gamma}$ make these functions transition functions for a [real line bundle](../../../../../../real-line-bundle.md) $L\to X$.

Choose local frames $e_\alpha$ with $e_\beta=g_{\alpha\beta}e_\alpha$. Then the local sections

$$
s|_{U_\alpha}=f_\alpha e_\alpha
$$

agree on overlaps and define a global section. Its zero set is exactly $Y$. Along $Y$, its vertical derivative is represented by the nonzero covector $df_\alpha$, so $s$ is transverse to the zero section, as in the [transverse intersection theorem](../../../../../../transverse-intersection-theorem.md). This is the [defining line bundle of a properly embedded hypersurface](../../../../../../defining-line-bundle-of-a-properly-embedded-hypersurface.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 115](../../../paper-115-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

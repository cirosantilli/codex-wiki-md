<h1 id="14f/solution">Solution</h1>

↑ **Parent:** [14F](../14f.md)

Close the real-line contour by a positively oriented upper semicircle of radius $R$, beyond every pole. The rational [function](../../../../../function-split.md) is $O(R^{-2})$ uniformly on that arc, and $|e^{iz}|=e^{-\Im z}\leq1$. Its arc [integral](../../../../../integral.md) is therefore $O(R^{-1})$ and vanishes. The real [integral](../../../../../integral.md) is absolutely convergent, while no pole lies on it. The residue theorem gives

$$
\boxed{\int_{-\infty}^{\infty}F(x)e^{ix}\,dx
=2\pi i\sum_{\Im z_j>0}\operatorname{Res}_{z=z_j}\bigl(F(z)e^{iz}\bigr).}
$$

Only actual poles contribute; any removable zero of the denominator has zero residue. The same contour proof covers poles of any order.

For the particular denominator, the upper poles are $a=1+i$ and $b=-1+i$. They are simple, with residues $e^{ia}/(4a^3)$ and $e^{ib}/(4b^3)$. Since

$$
\frac1{4a^3}=\frac{-1-i}{16},\qquad
\frac1{4b^3}=\frac{1-i}{16},
$$

their sum is

$$
\frac{e^{-1}}{16}\bigl[(-1-i)e^{i}+(1-i)e^{-i}\bigr]
=-\frac{i e^{-1}}8(\cos1+\sin1).
$$

Multiplication by $2\pi i$ gives the real answer. The sine part of the real-line [integral](../../../../../integral.md) is zero by oddness, so

$$
\boxed{\int_{-\infty}^{\infty}\frac{\cos x}{4+x^4}\,dx
=\frac{\pi}{4e}(\cos1+\sin1).}
$$

## ↑ Ancestors (10)

1. [14F](../14f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

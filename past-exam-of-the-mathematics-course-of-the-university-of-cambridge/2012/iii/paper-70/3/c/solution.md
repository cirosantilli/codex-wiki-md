<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [geometric series](../../../../../../geometric-series.md) formula and part (b) give

$$
E_n(f)=\sum_{k=m+1}^\infty3^{-k}=\frac12\,3^{-m},\qquad 5^m\le n<5^{m+1}.
$$

Put $\alpha=\log 3/\log 5$. Then $5^\alpha=3$, so $n^\alpha<3^{m+1}$ and

$$
\boxed{E_n(f)\le\frac{3}{2}n^{-\log 3/\log 5}.}
$$

This is the **largest possible decay exponent**: at $n=5^m$, an estimate with exponent $\beta>\alpha$ would require $\frac12\le c(3/5^\beta)^m$, whose right side tends to zero. Any smaller exponent also gives a valid weaker estimate. In fact $\frac12n^{-\alpha}\le E_n(f)<\frac32n^{-\alpha}$ for every $n\ge1$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

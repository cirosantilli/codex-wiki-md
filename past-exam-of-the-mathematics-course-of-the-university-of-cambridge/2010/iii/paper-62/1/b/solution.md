<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $j^{\underline m}=j(j-1)\cdots(j-m+1)$ for the [falling factorial](../../../../../../falling-factorial.md). At the sampling points, $f_{nm}(j/n)=n^{-m}j^{\underline m}$, which vanishes for $j<m$. For $j\ge m$, cancellation of the factorials gives

$$
j^{\underline m}\binom nj=\frac{n!}{(n-m)!}\binom{n-m}{j-m}=n^{\underline m}\binom{n-m}{j-m}.
$$

Insert this into the [Bernstein polynomial](../../../../../../bernstein-polynomial.md) and set $\ell=j-m$:

$$
\begin{aligned}
B_n(f_{nm},x)&=\frac{n^{\underline m}}{n^m}x^m\sum_{\ell=0}^{n-m}\binom{n-m}{\ell}x^\ell(1-x)^{n-m-\ell}\\
&=\frac{n^{\underline m}}{n^m}x^m=f_{nm}(1)x^m.
\end{aligned}
$$

The [binomial theorem](../../../../../../binomial-theorem.md) evaluates the remaining sum. For $m=0$, both sides equal one. This proves the **[Bernstein falling-factorial identity](../../../../../../bernstein-falling-factorial-identity.md) $B_n(f_{nm},x)=f_{nm}(1)x^m$**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

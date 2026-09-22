<h1 id="20/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Apply the [Leibniz rule](../../../../../leibniz-rule.md) to the $n$th [derivative](../../../../../derivative.md) in [Rodrigues' formula](../../../../../rodrigues-formula.md). If $j$ [derivatives](../../../../../derivative.md) fall on $e^{-x}$ and $n-j$ on $x^n$, the corresponding term is $\binom nj(-1)^je^{-x}(n!/j!)x^j$. Cancelling the prefactor gives

$$
\boxed{L_n(x)=\sum_{j=0}^n(-1)^j\binom nj\frac{x^j}{j!}}.
$$

The leading coefficient $(-1)^n/n!$ is nonzero, so this is a [polynomial](../../../../../polynomial-split.md) of degree exactly $n$. In particular, the requested coefficients in $L_{10}$ are

$$
\boxed{[x^{10}]L_{10}=\frac1{10!},\qquad [x^9]L_{10}=-\frac{10!}{(9!)^2}}.
$$

These are the ordinary [Laguerre polynomials](../../../../../laguerre-polynomial.md), with normalization $L_n(0)=1$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [20](../../20.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

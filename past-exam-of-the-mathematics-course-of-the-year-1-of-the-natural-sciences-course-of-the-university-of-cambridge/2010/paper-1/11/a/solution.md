<h1 id="11/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $f(x)=x^{1/4}$, the first two [derivatives](../../../../../derivative.md) are $f'(x)=\tfrac14x^{-3/4}$ and $f''(x)=-\tfrac3{16}x^{-7/4}$. At $16$ they give

$$
f(16)=2,\qquad f'(16)=\frac1{32},\qquad f''(16)=-\frac3{2048}.
$$

Use the first three [Taylor expansion](../../../../../taylor-expansion.md) terms with increment $17-16=1$:

$$
\boxed{17^{1/4}\approx2+\frac1{32}-\frac3{4096}=2.030517578125.}
$$

The positive third [derivative](../../../../../derivative.md) shows that this quadratic approximation underestimates the true value. The [Taylor remainder](../../../../../taylor-remainder.md) is at most $7/262144\approx2.67\times10^{-5}$, since $f^{(3)}(x)=(21/64)x^{-11/4}$ decreases on $[16,17]$ and the cubic remainder is $f^{(3)}(\xi)/6$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [11](../../11.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

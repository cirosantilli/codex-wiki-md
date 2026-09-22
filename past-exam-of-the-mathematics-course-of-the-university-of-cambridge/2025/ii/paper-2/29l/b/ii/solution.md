<h1 id="29l/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Under $H_0$, regardless of the unknown value of $\mu$,

$$
Q_n=\sum_{i=1}^n(X_i-\bar X)^2\sim\chi_{n-1}^2.
$$

Write $Q_n$ as a sum of $n-1$ independent squared standard normals. Since such a square has mean one and variance two, the central limit theorem gives

$$
\frac{Q_n-(n-1)}{\sqrt{2(n-1)}}\xrightarrow{d}N(0,1).
$$

Now

$$
\frac{Q_n-n}{\sqrt{2n}}
=\sqrt{\frac{n-1}{n}}
\frac{Q_n-(n-1)}{\sqrt{2(n-1)}}
-\frac1{\sqrt{2n}},
$$

so Slutsky's theorem makes this converge to $N(0,1)$. Squaring and using the continuous mapping theorem yields

$$
\boxed{T_n\xrightarrow{d}\chi_1^2.}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [29L](../../../29l.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

<h1 id="12d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The PDF defines this function using $\sin(1/x)$; the converted TeX contains a conflicting duplicate $\sin(1/2)$ before its later correct version. Use the PDF function. It is bounded by one and continuous at every positive $x$, although it is discontinuous at zero. Indeed the sequences $x_n=(\pi/2+2\pi n)^{-1}$ and $y_n=(3\pi/2+2\pi n)^{-1}$ tend to zero with function values $1$ and $-1$.

That single discontinuity does not prevent [Riemann integrability](../../../../../../riemann-integrable-function.md). Given $\varepsilon>0$, choose $0<\delta<\min\{1,\varepsilon/4\}$. The cell $[0,\delta]$ contributes at most $2\delta<\varepsilon/2$ to the difference between the [upper Darboux sum](../../../../../../upper-darboux-sum.md) and the [lower Darboux sum](../../../../../../lower-darboux-sum.md). On $[\delta,1]$ the function is uniformly continuous, so choose a partition there whose oscillation sum is less than $\varepsilon/2$, by the introductory proof. Joining that partition to the cell $[0,\delta]$ gives

$$
\boxed{U(g,P)-L(g,P)<2\delta+\varepsilon/2<\varepsilon.}
$$

Thus **the PDF's function is Riemann integrable despite its endpoint discontinuity**. This is a direct application of [bounded functions continuous away from one endpoint are Riemann integrable](../../../../../../bounded-functions-continuous-away-from-one-endpoint-are-riemann-integrable.md), proved here with the actual oscillation bound rather than an improper-integral argument.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [12D](../../12d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

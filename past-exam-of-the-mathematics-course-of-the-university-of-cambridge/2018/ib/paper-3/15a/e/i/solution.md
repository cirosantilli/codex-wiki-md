<h1 id="15a/e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a test function $f$, substitute $y=nx$ and use the [Taylor expansion](../../../../../../../taylor-expansion.md) $f(y/n)=f(0)+(y/n)f'(0)+O(n^{-2})$. Oddness removes the first term, while the [Gaussian integral](../../../../../../../gaussian-integral.md) gives $\int y^2e^{-y^2}dy=\sqrt\pi/2$. Hence

$$
\int n^3xe^{-n^2x^2}f(x)\,dx\longrightarrow\frac{\sqrt\pi}{2}f'(0)
=\left\langle-\frac{\sqrt\pi}{2}\delta',f\right\rangle.
$$

Therefore

$$
\boxed{n^3xe^{-n^2x^2}\longrightarrow-\frac{\sqrt\pi}{2}\delta'(x).}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [E](../../e.md)
3. [15A](../../../15a.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ib](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

<h1 id="12f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Normalization of the [probability density function](../../../../../../probability-density-function.md) gives

$$
1=A\int_0^{2\pi}(\pi-\phi/2)\,d\phi=A\pi^2,\qquad
\boxed{A=\pi^{-2}.}
$$

The first two [moments](../../../../../../moment.md) are

$$
\mathbb E\Phi=\frac1{\pi^2}\int_0^{2\pi}\phi(\pi-\phi/2)\,d\phi=\frac{2\pi}{3},\qquad
\mathbb E\Phi^2=\frac1{\pi^2}\int_0^{2\pi}\phi^2(\pi-\phi/2)\,d\phi=\frac{2\pi^2}{3}.
$$

Consequently

$$
\boxed{\mathbb E\Phi=\frac{2\pi}{3},\qquad
\operatorname{Var}\Phi=\frac{2\pi^2}{3}-\frac{4\pi^2}{9}=\frac{2\pi^2}{9}.}
$$

The [cumulative distribution function](../../../../../../cumulative-distribution-function.md) is $F(\phi)=\phi/\pi-\phi^2/(4\pi^2)=1-(1-\phi/(2\pi))^2$ on $[0,2\pi]$. For $U$ with the [uniform distribution](../../../../../../continuous-uniform-distribution.md) on $(0,1)$, [inverse transform sampling](../../../../../../inverse-transform-sampling.md) therefore uses

$$
\boxed{\Phi=2\pi\left(1-\sqrt{1-U}\right).}
$$

The inverse lies in the required interval and satisfies $F(\Phi)=U$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [12F](../../12f.md)
3. [Section II](../../section-ii.md)
4. [Paper 2](../../../paper-2-split.md)
5. [Ia](../../../split.md)
6. [2011](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)

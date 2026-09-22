<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [a](../a.md)

The [Cauchy derivative formula](../../../../cauchy-derivative-formula.md) says that if $f$ is [holomorphic](../../../../holomorphic-function-split.md) on a [neighbourhood](../../../../neighbourhood-mathematics.md) of a closed [disk](../../../../disk-mathematics.md) and $z_0$ is inside its positively oriented boundary [circle](../../../../circle.md) $\gamma$, then for $n\geq0$,

$$
\boxed{f^{(n)}(z_0)=\frac{n!}{2\pi i}\int_\gamma\frac{f(z)}{(z-z_0)^{n+1}}\,dz.}
$$

For $n=0$ this is the [Cauchy integral formula](../../../../cauchy-integral-formula.md). The same formula holds for a positively oriented simple closed [contour](../../../../complex-integration-contour.md) when $f$ is [holomorphic](../../../../holomorphic-function-split.md) on a [neighbourhood](../../../../neighbourhood-mathematics.md) of the contour and its enclosed region.

In the present problem the [unit circle](../../../../complex-unit-circle.md) and its closed interior lie inside $|z|<R$. Parametrize it by $z=e^{it}$, $0\leq t\leq2\pi$, so $dt=dz/(iz)$. For a positive integer $n$,

$$
\begin{aligned}
\int_0^{2\pi}f(e^{it})\cos(nt)\,dt
&=\frac1{2i}\int_{|z|=1}f(z)\bigl(z^{n-1}+z^{-n-1}\bigr)\,dz\\
&=\frac1{2i}\left(0+\frac{2\pi i}{n!}f^{(n)}(0)\right).
\end{aligned}
$$

The first [contour integral](../../../../contour-integral.md) is zero by the [Cauchy integral theorem](../../../../cauchy-s-integral-theorem.md), since $f(z)z^{n-1}$ is [holomorphic](../../../../holomorphic-function-split.md) on the [disk](../../../../disk-mathematics.md); the second is evaluated by the [Cauchy derivative formula](../../../../cauchy-derivative-formula.md). Therefore

$$
\boxed{\int_0^{2\pi}f(e^{it})\cos(nt)\,dt=\frac{\pi}{n!}f^{(n)}(0),\qquad n\geq1.}
$$

Taking $n=1$ gives the requested $\pi f'(0)$.

## ↑ Ancestors (12)

1. [a](../a.md)
2. [4](../../4.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../split.md)
5. [Metric spaces and complex analysis course of the University of Oxford](../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

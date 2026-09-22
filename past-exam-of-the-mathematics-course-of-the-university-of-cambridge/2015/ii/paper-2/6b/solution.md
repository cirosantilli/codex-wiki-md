<h1 id="6b/solution">Solution</h1>

↑ **Parent:** [6B](../6b.md)

[Analytic continuation](../../../../../analytic-continuation.md) extends a [holomorphic function](../../../../../holomorphic-function.md) by holomorphic elements agreeing on overlaps; along a path, a chain of overlapping neighbourhoods transports the initial element. The [identity theorem](../../../../../identity-theorem.md) makes compatible continuation unique on connected overlaps, although different paths can lead to different branches.

Choose the principal [complex logarithm](../../../../../complex-logarithm.md) and the slit domain $D=\mathbb C\setminus[1,\infty)$. On $D$, the function

$$
h(z)=-\frac{\operatorname{Log}(1-z)}z
$$

is holomorphic, with the removable value $h(0)=1$. The domain $D$ is simply connected, so $h$ has a primitive and its integral from $0$ to $z$ is independent of the path in $D$. For $|z|<1$, the uniformly convergent [power series](../../../../../power-series.md) on compact subdiscs gives

$$
f(z)=\int_0^zh(u)\,du=\int_0^z\sum_{n\geq1}\frac{u^{n-1}}n\,du=\sum_{n\geq1}\frac{z^n}{n^2}.
$$

Therefore **$f$ is a single-valued [analytic continuation](../../../../../analytic-continuation.md) of the [dilogarithm](../../../../../dilogarithm.md) to $\mathbb C\setminus[1,\infty)$**. The apparent problem at $0$ is removable; $1$ is a genuine branch point, even though the function has a finite one-sided limit there, because its derivative has a logarithmic singularity. Other cuts from $1$ to infinity give corresponding branches.

## ↑ Ancestors (10)

1. [6B](../6b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

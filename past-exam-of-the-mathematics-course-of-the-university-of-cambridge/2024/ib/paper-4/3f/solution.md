<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

A [function](../../../../../function-split.md) $f:U\to\mathbb C$ is holomorphic when it is complex [differentiable](../../../../../differentiable-function.md) at every point of the open connected set $U$. [Morera's theorem](../../../../../morera-s-theorem.md) states that a [continuous function](../../../../../continuous-function.md) on a domain is holomorphic if its [integral](../../../../../integral.md) around every triangle whose interior lies in the domain is zero.

The integrand $e^{tz}/(1+t^2)$ is continuous jointly in $(t,z)$ on $[0,1]\times\mathbb C$, so the displayed [integral](../../../../../integral.md) defines a [continuous function](../../../../../continuous-function.md). For any triangle $T$, Fubini's theorem and the Cauchy [integral](../../../../../integral.md) theorem give

$$
\int_{\partial T}f(z)\,dz
=\int_0^1\frac1{1+t^2}
\left(\int_{\partial T}e^{tz}\,dz\right)dt
=0.
$$

Morera's theorem therefore proves that $f$ is entire.

The [function](../../../../../function-split.md) $1/z$ is holomorphic on $\mathbb C\setminus\{0\}$ but has no antiderivative there, because an antiderivative would integrate to zero around every closed curve whereas

$$
\int_{|z|=1}\frac{dz}{z}=2\pi i.
$$

This is the standard [period obstruction to a holomorphic antiderivative](../../../../../period-obstruction-to-a-holomorphic-antiderivative.md).

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Taking $k_2\to k_1=k$ in the preceding [probability density](../../../../probability-density.md) gives $p_2(t)=k^2te^{-kt}$. Convolving once more with an independent [exponential distribution](../../../../exponential-distribution.md) gives

$$
p_3(t)=\int_0^t k^2s e^{-ks}ke^{-k(t-s)}\,ds=\frac{k^3t^2}{2}e^{-kt}.
$$

More generally, suppose $p_n(s)=k^ns^{n-1}e^{-ks}/(n-1)!$. Then

$$
p_{n+1}(t)=\frac{k^{n+1}e^{-kt}}{(n-1)!}\int_0^t s^{n-1}\,ds
=\frac{k^{n+1}t^n e^{-kt}}{n!}.
$$

Since $p_1(t)=ke^{-kt}$, this proves the [Erlang distribution](../../../../erlang-distribution.md) formula by [mathematical induction](../../../../mathematical-induction.md). Normalization follows either from the [convolution](../../../../convolution.md) or $\int_0^\infty t^{n-1}e^{-kt}\,dt=(n-1)!/k^n$.

$$
\boxed{p_n(t)=\frac{k^nt^{n-1}e^{-kt}}{(n-1)!},\qquad
\Pr(t<T<t+dt)=p_n(t)dt+o(dt),\qquad
 t_{\rm mode}=\frac{n-1}{k}.}
$$

For $n>1$, differentiating $\log p_n$ gives $(n-1)/t-k=0$, and the derivative changes from positive to negative. For $n=1$ the maximum occurs at the boundary $t=0$. **Source dimensional qualification:** the printed expression without $dt$ is a [probability density](../../../../probability-density.md), with units of inverse time; it cannot itself be a dimensionless interval [probability](../../../../probability.md).

In the right panel of the original illustration in [d](../../2/d.md), $p_2/k$ rises linearly near zero and peaks at $kt=1$ with height $1/e$. The curve $p_3/k$ rises quadratically and peaks later, at $kt=2$, with lower height $2e^{-2}$. Both have exponential tails, but the latter has the larger [expected value](../../../../expected-value-split.md) $3/k$ and [variance](../../../../variance-split.md) $3/k^2$, compared with $2/k$ and $2/k^2$. This distinguishes both the onset and the width of the requested sketches.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [5](../../5.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

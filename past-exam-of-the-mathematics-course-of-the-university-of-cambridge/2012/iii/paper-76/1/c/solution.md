<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For small $x$, use $u=\cosh t$ to write the defining [oscillatory integral](../../../../../../oscillatory-integral.md) as

$$
I(x)=\int_1^\infty\frac{\cos(xu)}{\sqrt{u^2-1}}\,du=\int_1^\infty\frac{\cos(xu)}u\,du+\int_1^\infty\cos(xu)\left(\frac1{\sqrt{u^2-1}}-\frac1u\right)du.
$$

The first integral is $-\operatorname{Ci}(x)$, where the [cosine integral](../../../../../../cosine-integral.md) satisfies $\operatorname{Ci}(x)=\gamma_E+\log x+O(x^2)$. Its logarithm follows by integrating the $1/x$ singularity of its derivative; its conventional constant is the [Euler--Mascheroni constant](../../../../../../euler-s-constant.md). The primary normalization is given by [https://dlmf.nist.gov/6.6.E6](https://dlmf.nist.gov/6.6.E6) .

The second integrand has an integrable inverse-square-root endpoint singularity and an $O(u^{-3})$ tail. The [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) therefore gives its limit

$$
\int_1^\infty\left(\frac1{\sqrt{u^2-1}}-\frac1u\right)du=\lim_{L\to\infty}(\operatorname{arcosh}L-\log L)=\log2.
$$

Splitting at $u=1/x$ and using $|1-\cos(xu)|\le\min(x^2u^2/2,2)$ also bounds its error by $O(x^2|\log x|)$. Thus

$$
\boxed{g(x)=\frac2\pi\left(\log\frac x2+\gamma_E\right)+O(x^2|\log x|),\qquad x\downarrow0.}
$$

In particular, the leading term is $(2/\pi)\log x$.

For large $x$, the phase $\cosh t$ has its only stationary point at the endpoint $t=0$. Its expansion is $1+t^2/2+O(t^4)$, so the contributing width is $t=O(x^{-1/2})$. The endpoint [stationary phase method](../../../../../../stationary-phase-method.md) and the [Fresnel integral](../../../../../../fresnel-integral.md) yield

$$
\int_0^\infty e^{ix\cosh t}dt\sim e^{ix}\int_0^\infty e^{ixt^2/2}dt=e^{i(x+\pi/4)}\sqrt{\frac\pi{2x}}.
$$

A smooth cutoff near the endpoint justifies this local replacement; the remaining nonstationary tail can be integrated by parts, with no stationary contribution at infinity. Taking the real part gives the [Bessel function of the second kind](../../../../../../bessel-function-of-the-second-kind.md) asymptotic

$$
\boxed{g(x)=\sqrt{\frac2{\pi x}}\sin(x-\pi/4)+O(x^{-3/2}),\qquad x\to\infty.}
$$

The additive error formulation remains meaningful near zeros of the leading oscillation. Both limits were derived from the given integral, rather than identifying a special function and merely quoting its asymptotics.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

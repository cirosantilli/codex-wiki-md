<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Watson's lemma](../../../../../../watson-s-lemma.md) applies to Laplace-type endpoint integrals such as $\int_0^b e^{-\lambda t}f(t)\,dt$ as $\lambda\to+\infty$, when $f$ has a local algebraic expansion $f(t)\sim\sum_jc_jt^{p+j-1}$ with $p>0$ and suitable integrability or exponential-growth control away from the endpoint. Each term contributes $c_j\Gamma(p+j)\lambda^{-p-j}$. The exponential selects a neighborhood of $t=0$.

[Laplace method](../../../../../../laplace-s-method.md) instead treats $\int_a^b g(t)e^{\lambda\phi(t)}\,dt$ by locating the dominant maxima of a real phase $\phi$. A smooth nondegenerate interior maximum produces a neighborhood governed by a [Gaussian function](../../../../../../gaussian-function.md) of width $\lambda^{-1/2}$; endpoint or degenerate maxima require their corresponding local scaling. Contributions away from a strict dominant maximum must be smaller. These methods overlap after suitable changes of variable, but their usual starting forms emphasize an endpoint amplitude expansion and an exponential maximum, respectively.

For the [Gamma function](../../../../../../gamma-function.md), put $t=xu$. Then

$$
\Gamma(x)=x^x\int_0^\infty u^{-1}e^{x(\log u-u)}\,du.
$$

The phase has its unique maximum at $u=1$, with value $-1$ and second derivative $-1$. Set $u=1+s/\sqrt x$. Near this maximum,

$$
x(\log u-u)=-x-\frac{s^2}2+\frac{s^3}{3\sqrt x}-\frac{s^4}{4x}+\cdots,\qquad
u^{-1}=1-\frac{s}{\sqrt x}+\frac{s^2}{x}+\cdots.
$$

Combining the amplitude and exponential expansions in [Laplace method](../../../../../../laplace-s-method.md) gives

$$
\Gamma(x)\sim x^{x-1/2}e^{-x}\int_{-\infty}^{\infty}e^{-s^2/2}\left[1+\frac{s^3/3-s}{\sqrt x}+\frac{s^2-7s^4/12+s^6/18}{x}+\cdots\right]ds.
$$

Localization near $u=1$ justifies extending the limits for the [Gaussian integral](../../../../../../gaussian-integral.md); the distant endpoint is not being expanded uniformly by this local series. Odd terms integrate to zero. The moments of the [Gaussian integral](../../../../../../gaussian-integral.md) satisfy $I_1=I_0$, $I_2=3I_0$, $I_3=15I_0$, so the relative correction is

$$
1-\frac7{12}\cdot3+\frac1{18}\cdot15=\frac1{12}.
$$

The two terms of the [Stirling formula](../../../../../../stirling-formula.md), obtained by the [Stirling correction by Gaussian moments](../../../../../../stirling-correction-by-gaussian-moments.md), are therefore

$$
\boxed{\Gamma(x)=\sqrt{2\pi}\,x^{x-1/2}e^{-x}\left(1+\frac1{12x}+O(x^{-2})\right),\qquad x\to+\infty}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="30b/solution">Solution</h1>

↑ **Parent:** [30B](../30b.md)

For the [Laplace method](../../../../../laplace-s-method.md), under the usual regularity ($p$ continuous at zero and $q$ sufficiently smooth near its isolated minimum), write $q(t)=q(0)+q''(0)t^2/2+o(t^2)$. On any interval bounded away from zero, [continuity](../../../../../continuous-function.md) and uniqueness of the minimum give a positive gap in $q$, making that contribution exponentially smaller. Set $t=s/\sqrt{x}$ near zero. The leading integral is

$$
I(x)=e^{-xq(0)}x^{-1/2}\left[p(0)\int_0^\infty e^{-q''(0)s^2/2}ds+o(1)\right].
$$

A local quadratic lower bound on $q-q(0)$ justifies dominated convergence after this rescaling. Thus, when $p(0)\ne0$,

$$
\boxed{I(x)\sim p(0)e^{-xq(0)}\sqrt{\frac{\pi}{2xq''(0)}}.}
$$

If $p(0)=0$, the displayed coefficient vanishes and further local terms of $p$ determine the first nonzero asymptotic term; one must not interpret a zero coefficient as an [asymptotic equivalence](../../../../../asymptotic-equivalence.md).

For the first Bessel integral, take $q(\theta)=-\cos\theta$, $p(\theta)=\cos(\nu\theta)$. The endpoint minimum is $q(0)=-1$, $q''(0)=1$, $p(0)=1$, so after dividing by $\pi$ its leading term is $e^x/\sqrt{2\pi x}$.

For the second integral, $\cosh t\geq1+t^2/2$ gives, for fixed real $\nu$,

$$
\left|\int_0^\infty e^{-x\cosh t-\nu t}dt\right|\leq e^{-x}\int_0^\infty e^{-xt^2/2+|\nu|t}dt=O(e^{-x}x^{-1/2}).
$$

Completing the square proves the last bound for large $x$. It is exponentially smaller than the first integral; the fixed prefactor $\sin(\nu\pi)$ does not change this. Therefore

$$
\boxed{I_\nu(x)\sim\frac{e^x}{\sqrt{2\pi x}}\quad(x\to+\infty,\ \nu\text{ fixed}).}
$$

## ↑ Ancestors (10)

1. [30B](../30b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

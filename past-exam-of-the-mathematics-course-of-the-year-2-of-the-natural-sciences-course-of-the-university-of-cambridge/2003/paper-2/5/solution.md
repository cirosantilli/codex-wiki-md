<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The [Laplace transform](../../../../laplace-transform.md) is $\overline f(p)=\int_0^\infty e^{-pt}f(t)dt$ wherever it converges. For sufficiently large $\operatorname{Re}p$, suitable exponential bounds justify [integration by parts](../../../../integration-by-parts.md) and [differentiation under the integral sign](../../../../differentiation-under-the-integral-sign.md), giving

$$
\boxed{\mathcal L[f'](p)=p\overline f(p)-f(0^+),\qquad\mathcal L[tf](p)=-\overline f'(p).}
$$

For a nonnegative [integer](../../../../integer-split.md) $n$ and real $p>0$, substitute $u=pt$ in the [gamma integral](../../../../gamma-integral.md). The result extends holomorphically to $\operatorname{Re}p>0$, giving

$$
\boxed{\mathcal L[t^n](p)=\frac{n!}{p^{n+1}},\qquad\operatorname{Re}p>0.}
$$

This also follows recursively from the second identity, starting with $\mathcal L[1]=1/p$.

Put $G=\overline g$, $g_0=g(0^+)$ and $g_1=g'(0^+)$. For a solution with finite initial values and the required transform bounds, the transformed equation is

$$
-\frac d{dp}(p^2G-pg_0-g_1)+(pG-g_0)+\frac d{dp}(pG-g_0)+2G=0.
$$

The initial-value terms cancel, leaving $(p-p^2)G'+(3-p)G=0$. On the real interval $p>1$, a nonzero solution satisfies

$$
\frac{G'}G=\frac{3-p}{p^2-p}=-\frac3p+\frac2{p-1}.
$$

Integration gives $G=C(p-1)^2/p^3=C(1/p-2/p^2+1/p^3)$. Inverting term by term yields

$$
\boxed{g(t)=C\left(1-2t+\frac{t^2}2\right).}
$$

Taking $C=1$ gives a nonzero solution, verified by direct substitution. It is $L_2(t)$, and the rational transform agrees with the general [Laplace transform of a Laguerre polynomial](../../../../laplace-transform-of-a-laguerre-polynomial.md). No claim about solutions with singular initial behavior is needed to produce this regular solution.

## ↑ Ancestors (12)

1. [5](../5.md)
2. [Paper 2](../../paper-2-split.md)
3. [2003](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

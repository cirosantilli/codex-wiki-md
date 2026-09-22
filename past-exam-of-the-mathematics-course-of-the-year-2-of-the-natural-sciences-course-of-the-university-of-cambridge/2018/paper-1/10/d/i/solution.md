<h1 id="10/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the proposed trial profile, $R'=-qr^{q-1}$. Its weighted [energy](../../../../../../energy-split.md) is

$$
\int_0^1r^{n+1}R'^2\,dr=q^2\int_0^1r^{n+2q-1}\,dr=\frac{q^2}{n+2q}.
$$

The squared [weighted norm](../../../../../../weighted-norm.md) is

$$
\int_0^1r(1-r^q)^2\,dr
=\frac12-\frac2{q+2}+\frac1{2q+2}
=\frac{q^2}{2(q+1)(q+2)}.
$$

Both are finite for $q>0$ and $n\geq0$, and $R(1)=0$. Therefore the [Rayleigh-Ritz variational principle](../../../../../../rayleigh-ritz-variational-principle.md) gives

$$
\boxed{\nu_{\mathrm{trial}}(q,n)=\frac{2(q+1)(q+2)}{n+2q},\qquad
\inf\operatorname{spec}\leq\nu_{\mathrm{trial}}}.
$$

When a [fundamental diffusion mode](../../../../../../fundamental-diffusion-mode.md) exists, its decay rate is the infimum and is bounded above by this expression.

The existence qualification matters for the full range of $n$ printed in the question. For $n>2$, trial functions concentrated within radius $\varepsilon$ have quotient proportional to $\varepsilon^{n-2}$, proving the [loss of a spectral gap under strongly degenerate radial diffusion](../../../../../../loss-of-a-spectral-gap-under-strongly-degenerate-radial-diffusion.md). The infimum is zero and is not attained, because zero [energy](../../../../../../energy-split.md) together with $R(1)=0$ forces the zero function. Thus there is no positive lowest-mode decay rate in that case. Even at $n=2$, the mode equation is $r^2R''+3rR'+\nu R=0$: its characteristic powers are $r^{-1\pm\sqrt{1-\nu}}$, and for $\nu>0$ every nonzero solution is unbounded at the centre. Hence the asserted bounded fundamental mode cannot be assumed for all $n\geq0$. The trial quotient remains valid, and the next part's $n=0$ case has the usual fundamental mode.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [D](../../d.md)
3. [10](../../../10.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)

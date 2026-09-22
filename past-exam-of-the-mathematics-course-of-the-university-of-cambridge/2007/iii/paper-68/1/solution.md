<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the [method of multiple scales](../../../../../method-of-multiple-scales.md), treating $t$ and $\tau=t/\epsilon$ as independent variables, so differentiation becomes $\partial_t+\epsilon^{-1}\partial_\tau$. Write $L=\partial_x^2-\ell^2$ and average over a fast period $2\pi/|\omega|$, with $\omega\ne0$. The fluctuations can depend slowly on $x,t$ as well as periodically on $\tau$. The $\epsilon^{-1}$ balance in the [poloidal magnetic field](../../../../../poloidal-magnetic-field.md) potential equation is

$$
\partial_\tau\widetilde A=\alpha_0\sin(\omega\tau)\overline B.
$$

Integrating and imposing zero fast average determines

$$
\widetilde A=-\frac{\alpha_0}{\omega}\cos(\omega\tau)\overline B.
$$

At order one, the [toroidal magnetic field](../../../../../toroidal-magnetic-field.md) equation is $\partial_t\overline B+\partial_\tau\widetilde B=\Omega\partial_x(\overline A+\widetilde A)+L\overline B$. Its average and fluctuating parts give, respectively,

$$
\partial_t\overline B=\Omega\partial_x\overline A+L\overline B,\qquad
\partial_\tau\widetilde B=\Omega\partial_x\widetilde A.
$$

Consequently the zero-average fluctuation is

$$
\widetilde B=-\frac{\Omega\alpha_0}{\omega^2}\sin(\omega\tau)\partial_x\overline B.
$$

The order-one averaged [poloidal magnetic field](../../../../../poloidal-magnetic-field.md) potential equation retains the correlation between the fluctuating [alpha effect](../../../../../alpha-effect.md) and the fluctuating [toroidal magnetic field](../../../../../toroidal-magnetic-field.md). Although alpha has zero average, its product with the magnetic fluctuation does not:

$$
\overline{\widetilde\alpha\widetilde B}
=-\frac{\Omega\alpha_0^2}{\omega^2}\overline{\sin^2(\omega\tau)}\partial_x\overline B
=-C\partial_x\overline B,\qquad
\boxed{C=\frac{\Omega\alpha_0^2}{2\omega^2}}.
$$

Thus the [rapidly fluctuating alpha effect](../../../../../rapidly-fluctuating-alpha-effect.md) produces the leading averaged equations

$$
\boxed{\partial_t\overline A=-C\partial_x\overline B+L\overline A,\qquad
\partial_t\overline B=\Omega\partial_x\overline A+L\overline B}.
$$

A higher-order zero-average correction to $A$ accommodates the remaining fast order-one terms; it does not alter this leading averaged balance. These equations describe the small-$\epsilon$ limit, rather than an exact finite-$\epsilon$ identity.

For a [Fourier mode](../../../../../fourier-mode.md), let $(\overline A,\overline B)=(a,b)e^{ikx+\sigma t}$ and put $d=k^2+\ell^2$. Then $(\sigma+d)a=-ikCb$ and $(\sigma+d)b=ik\Omega a$. Their determinant gives the [dispersion relation](../../../../../dispersion-relation.md)

$$
(\sigma+d)^2=\Omega Ck^2,\qquad
\boxed{\sigma_\pm=-k^2-\ell^2\pm|k|\sqrt{\Omega C}}.
$$

Here $\Omega C=\Omega^2\alpha_0^2/(2\omega^2)\ge0$, so both [growth rates](../../../../../growth-rate.md) are real. For a prescribed nonzero [wavenumber](../../../../../wavenumber.md), growth requires $\Omega C>(k^2+\ell^2)^2/k^2$. If real [wavenumbers](../../../../../wavenumber.md) can be chosen freely, the largest [growth rate](../../../../../growth-rate.md) occurs at $|k|=\sqrt{\Omega C}/2$ and is $\Omega C/4-\ell^2$. Hence **growing averaged modes exist precisely when**

$$
\boxed{\Omega C>4\ell^2}.
$$

A bounded or periodic spatial domain instead requires an admissible [wavenumber](../../../../../wavenumber.md) satisfying the preceding mode-by-mode inequality.

The physical feedback differs from an ordinary [Parker dynamo wave](../../../../../parker-dynamo-wave.md). A constant [alpha effect](../../../../../alpha-effect.md) couples $B$ directly into $A$, while the [Omega effect](../../../../../omega-effect.md) differentiates $A$ once, producing the factor $ik\alpha\Omega$ responsible for an oscillatory phase. Here the fast [alpha effect](../../../../../alpha-effect.md) first creates a potential fluctuation in temporal quadrature; shear creates a magnetic fluctuation correlated with alpha. The averaged feedback is consequently proportional to $-\partial_x\overline B$. Combining its spatial derivative with the derivative in the [Omega effect](../../../../../omega-effect.md) gives the real positive factor $\Omega Ck^2$. In fact $(\partial_t-L)^2\overline B=-\Omega C\partial_x^2\overline B$. The resulting growing fields have fixed spatial phase, so **the leading averaged pattern grows without travelling**. Fast within-period oscillations of the original fields remain present.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 68](../../paper-68-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

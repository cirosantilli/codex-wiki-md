<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take $0<r_1<r_2$ and positive mean [kinematic viscosity](../../../../../../../kinematic-viscosity.md) $\bar\nu$. The [steady state](../../../../../../../steady-state.md) of the supplied [viscous evolution of an accretion disk](../../../../../../../viscous-evolution-of-an-accretion-disk.md) equation satisfies $\mathcal F'=-2\pi rS(r)$. The outer no-flux condition therefore gives

$$
\mathcal F(r)=2\pi\int_r^{r_2}vS(v)\,dv.
$$

Positive $S$ produces positive inward [accretion rate](../../../../../../../accretion-rate.md) in this sign convention. Set $Y=r^{1/2}\bar\nu\Sigma$. In a [Keplerian disk](../../../../../../../keplerian-disk.md), the [viscous torque in an accretion disk](../../../../../../../viscous-torque-in-an-accretion-disk.md) is proportional to $Y$, so the [zero-torque inner boundary condition](../../../../../../../zero-torque-inner-boundary-condition.md) gives $Y(r_1)=0$. Since $Y'=\mathcal F/(6\pi r^{1/2})$, a second integration yields

$$
\boxed{\Sigma(r)=\frac{1}{3\bar\nu(r)r^{1/2}}\int_{r_1}^{r}u^{-1/2}\left[\int_u^{r_2}vS(v)\,dv\right]du.}
$$

This is the [steady viscous disk supplied by a radial source](../../../../../../../steady-viscous-disk-supplied-by-a-radial-source.md). It does not require $\bar\nu$ to be independent of radius: the equation directly determines $\bar\nu\Sigma$. If viscosity depends on the local thermodynamic state, the displayed formula is an implicit relation completed by a separate closure. For nonnegative integrable $S$ it gives nonnegative [surface density of a disk](../../../../../../../surface-density-of-a-disk.md), and the inner [accretion rate](../../../../../../../accretion-rate.md) equals the total supplied mass per unit time, $2\pi\int_{r_1}^{r_2}rS(r)dr$. Differentiating both nested integrals recovers the flux and the differential equation.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 321](../../../../paper-321-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

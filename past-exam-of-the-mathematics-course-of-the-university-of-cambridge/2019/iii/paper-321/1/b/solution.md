<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In a [steady state](../../../../../../steady-state.md), [mass conservation](../../../../../../mass-conservation.md) makes $\mathcal F$ independent of radius. Taking the [accretion rate](../../../../../../accretion-rate.md) $\dot M>0$ for inward flow gives $\mathcal F=-\dot M$. The [conservation of angular momentum](../../../../../../conservation-of-angular-momentum.md) equation then makes $-\dot M h+\mathcal G$ constant. The [zero-torque inner boundary condition](../../../../../../zero-torque-inner-boundary-condition.md) fixes this constant to $-\dot M h_{\rm in}$, so

$$
\mathcal G=\dot M(h-h_{\rm in}).
$$

The [viscous torque in an accretion disk](../../../../../../viscous-torque-in-an-accretion-disk.md) is $\mathcal G=-2\pi r^3\bar\nu\Sigma\Omega'=2\pi qh\bar\nu\Sigma$. Combining these expressions gives the [steady accretion disk with arbitrary rotation law](../../../../../../steady-accretion-disk-with-arbitrary-rotation-law.md)

$$
\bar\nu\Sigma=\frac{\dot M}{2\pi q}
\left(1-\frac{h_{\rm in}}h\right).
$$

For $x=r/R_g$, the [Paczyński-Wiita circular orbit](../../../../../../paczynski-wiita-circular-orbit.md) formulas give

$$
\frac3{2q}=\frac{x-2}{x-2/3},\qquad
\frac{h_{\rm in}}h=\frac{3\sqrt3(x-2)}{\sqrt2\,x^{3/2}}.
$$

Consequently

$$
\boxed{\bar\nu\Sigma=\frac{f\dot M}{3\pi}},\qquad
\boxed{f=\frac{x-2}{x-2/3}
\left[1-\frac{3\sqrt3(x-2)}{\sqrt2\,x\sqrt x}\right]}.
$$

In particular, $f(6)=0$ and $f\to1$ far from the black hole, recovering the outer [Keplerian accretion disk](../../../../../../keplerian-accretion-disk.md).

Inside the [innermost stable circular orbit](../../../../../../innermost-stable-circular-orbit.md), the gas enters the [plunging region of a black-hole accretion disk](../../../../../../plunging-region-of-a-black-hole-accretion-disk.md). Its rapid inward motion leaves little time for stresses to exchange [angular momentum](../../../../../../angular-momentum.md), motivating the [zero-torque inner boundary condition](../../../../../../zero-torque-inner-boundary-condition.md). This is a thin-disc approximation; a strong magnetic stress could change it.

Matter supplied from very large radius has negligible [specific orbital energy](../../../../../../specific-orbital-energy.md), while matter crossing the inner edge carries $\varepsilon_{\rm in}=-\eta c^2$. With zero inner torque, no energy is supplied by a stress at that edge. If the heat released outside it escapes by [radiative transfer](../../../../../../radiative-transfer.md), rather than being lost through inward [advection](../../../../../../advection.md), the integrated [conservation of energy](../../../../../../conservation-of-energy.md) balance gives

$$
\boxed{L_{\rm disc}=-\dot M\varepsilon_{\rm in}=\eta\dot M c^2=\frac{\dot M c^2}{16}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 321](../../../paper-321-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

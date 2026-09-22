<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

First analyze the supplied [normal form](../../../../../../normal-form-dynamical-systems.md) as a [dynamical system](../../../../../../dynamical-system.md) in its own right. Its [equilibrium points](../../../../../../equilibrium-point-of-a-dynamical-system.md) are $O=(0,0)$ and, for $\mu_2>0$, $S_\pm=(\pm\sqrt{\mu_2},0)$. At $O$, the [trace](../../../../../../matrix-trace.md) is $\mu_1$ and the [determinant](../../../../../../determinant.md) is $\mu_2$. At $S_\pm$, the [determinant](../../../../../../determinant.md) is $-2\mu_2$, so both are [saddle equilibria](../../../../../../saddle-equilibrium.md). Thus $\mu_2=0$ is the [pitchfork bifurcation](../../../../../../pitchfork-bifurcation-normal-form.md) curve, and $\mu_1=0,\mu_2>0$ is the [Hopf bifurcation](../../../../../../hopf-bifurcation.md) curve. With the allowed supercritical [Hopf bifurcation](../../../../../../hopf-bifurcation.md), an attracting [limit cycle](../../../../../../limit-cycle.md) is born on $\mu_1>0$ around the repelling origin.

The [Hamiltonian](../../../../../../hamiltonian.md) $H=y^2/2+\mu_2x^2/2-x^4/4$ obeys $\dot H=(\mu_1-x^2)y^2$. Set $s=\mu_2>0$, $x=\sqrt s X$, $y=sY$, $\tau=\sqrt s\,t$, and $\mu_1=cs$. The limiting [Hamiltonian system](../../../../../../hamiltonian-system.md) has two oppositely directed [heteroclinic orbits](../../../../../../heteroclinic-orbit.md) with $Y=\pm(1-X^2)/\sqrt2$ for $-1<X<1$. The [Melnikov energy-balance method](../../../../../../melnikov-energy-balance-method.md) gives

$$
\int_{-1}^1(c-X^2)(1-X^2)\,dX=\frac43c-\frac4{15}.
$$

Its unique simple zero gives a [heteroclinic cycle](../../../../../../heteroclinic-cycle.md) curve

$$
\boxed{\mu_1=h(\mu_2),\qquad h(s)=s/5+o(s),\quad s>0.}
$$

The two connections occur on the same curve because reflection interchanges them. The attracting [limit cycle](../../../../../../limit-cycle.md) grows toward this [heteroclinic cycle](../../../../../../heteroclinic-cycle.md), then disappears. In the small unfolding neighborhood there is one such connection curve, rather than two independently split curves. There are no nearby [homoclinic orbits](../../../../../../homoclinic-orbit.md) replacing it: the two equal-height outer saddles are the relevant separatrix endpoints.

This calculation transfers to the original equations only if the asserted reduction is valid. The cubic calculation in part (c) shows it is not valid for the printed coefficients. Nevertheless, the claim of a single nearby [global bifurcation](../../../../../../global-bifurcation.md) curve for the original equations can be proved independently. Put $\eta=-(\kappa+1)>0$, $\lambda=3+\eta^2L$, $x=\phi=\sqrt\eta X$, $y=\dot\phi=\eta Y$, and $\tau=\sqrt\eta\,t$. Eliminating $\theta$ using $\sin q=(y+\sin2x)/(\cos2x-\kappa)$ produces

$$
\begin{aligned}
X'&=Y,\\
Y'&=-2X+8X^3+\eta\left(\frac{10}{3}X^3+2LX-16X^5-4XY^2\right)\\
&\quad+\eta^{3/2}Y\left(L+6X^2-12X^4-\frac12Y^2\right)+O(\eta^2).
\end{aligned}
$$

The order-$\eta$ correction is reversible and has no first-order separatrix energy imbalance. On the limiting positive connection, $-1/2<X<1/2$ and $Y=1/2-2X^2$. The first dissipative balance is

$$
\int_{-1/2}^{1/2}\left(L-\frac18+7X^2-14X^4\right)\left(\frac12-2X^2\right)\,dX
=\frac13\left(L+\frac3{20}\right).
$$

Again the zero is simple, and reflection makes the two [heteroclinic orbits](../../../../../../heteroclinic-orbit.md) simultaneous. Hence the actual original equations have the unique local connection curve

$$
\boxed{\lambda=3-\frac3{20}(\kappa+1)^2+o((\kappa+1)^2),\qquad\kappa<-1.}
$$

The unstable [limit cycle](../../../../../../limit-cycle.md) on the subcritical [Hopf bifurcation](../../../../../../hopf-bifurcation.md) side reaches this curve. Thus the original system still has one nearby global connection curve, but its tangency and cycle stability differ from those of the supplied assumed cubic [normal form](../../../../../../normal-form-dynamical-systems.md). These statements concern connections contained in the shrinking neighborhood of $P_1$; they do not exclude unrelated distant [global bifurcations](../../../../../../global-bifurcation.md) elsewhere on the sphere.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

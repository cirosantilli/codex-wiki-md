<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the steady positive-velocity branch, conservation of [buoyancy flux](../../../../../../buoyancy-flux.md) gives $bhu=F_0$. Substituting into the other two balances gives

$$
(hu)'=\alpha u,\qquad
\left(hu^2+\frac{F_0h}{2u}\cos\theta\right)'=\frac{F_0}{u}\sin\theta.
$$

Use a [power-law ansatz](../../../../../../power-law-ansatz.md) $h=Cx^p$, $u=Dx^q$. The entrainment balance forces $p=1$ and $C(1+q)=\alpha$. The momentum powers are $x^{2q}$, $x^{-q}$ and $x^{-q}$, so the nonzero inertial branch has $q=0$. Therefore the [constant-speed entraining gravity current on a slope](../../../../../../constant-speed-entraining-gravity-current-on-a-slope.md) is

$$
\boxed{h=\alpha x,\qquad
u=\left[\frac{F_0}{\alpha}\left(\sin\theta-\frac{\alpha}{2}\cos\theta\right)\right]^{1/3},\qquad
\rho-\rho_0=\frac{\rho_0F_0}{g\alpha ux}.}
$$

Its positive speed requires $\tan\theta>\alpha/2$ for $\theta<\pi/2$. In the shallow, strictly hyperbolic range this means

$$
\boxed{\arctan(\alpha/2)<\theta<\pi/2,\qquad \alpha\ll1.}
$$

The same steady integral balances have a formal vertical-plume limit at $\theta=\pi/2$, although their time-dependent system then loses strict [hyperbolicity](../../../../../../hyperbolicity.md). At the lower threshold the assumed positive-flux, finite-speed solution fails.

The line source is singular: $h,u h$ and the momentum flux tend to zero, but $b$ diverges as $x\downarrow0$. Thus this is a downstream ideal-source solution, valid only far enough away that $b/g\ll1$ and the [Boussinesq approximation](../../../../../../boussinesq-approximation.md) and [top-hat plume model](../../../../../../top-hat-plume-model.md) hold. It does not describe the immediate source region.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

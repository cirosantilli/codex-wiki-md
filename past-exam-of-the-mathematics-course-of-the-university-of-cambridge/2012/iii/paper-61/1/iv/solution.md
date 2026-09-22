<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The required [pressure](../../../../../../pressure.md) integral uses $\int_0^1(1-x^2)^4dx=128/315$. With $\Sigma=(32/35)\rho_0H$ and $p_0/\rho_0=\Omega^2H^2/8$,

$$
\int_{-H}^Hp\,dz=\frac{256}{315}p_0H=\frac{\Sigma\Omega^2H^2}{9}.
$$

The [vertically averaged alpha closure for a mixed-pressure layer](../../../../../../vertically-averaged-alpha-closure-for-a-mixed-pressure-layer.md) therefore gives

$$
\boxed{\bar\nu=\frac{\alpha H^2\Omega}{9}.}
$$

The height-integrated [dynamic viscosity](../../../../../../dynamic-viscosity.md) is $2H\mu=8cH\lambda/[9\kappa(1+\lambda)]$. Equate it to $\bar\nu\Sigma$ to obtain

$$
\boxed{\frac\lambda{1+\lambda}=\frac{\alpha H\Omega\kappa\Sigma}{8c}.}
$$

These are integrated equalities, not an imposed pointwise relation $\mu(z)\propto p(z)$.

Now keep $\alpha$, the [opacity](../../../../../../opacity.md) and molecular constants independent of radius, and use [Keplerian rotation](../../../../../../keplerian-disk.md) $\Omega\propto r^{-3/2}$. In the gas-dominated limit, $\lambda\ll1$ but positive, the last equality gives $\lambda\propto H\Omega\Sigma$. The column-density relation gives $\lambda\Sigma\propto H^7\Omega^6$. Eliminating $\lambda$ yields $H^6\propto\Sigma^2\Omega^{-5}$, whence

$$
\boxed{\bar\nu\propto\Sigma^{2/3}\Omega^{-2/3}\propto r\Sigma^{2/3}\qquad(\lambda\ll1).}
$$

This is the [gas-pressure branch of a mixed-pressure alpha disk](../../../../../../gas-pressure-branch-of-a-mixed-pressure-alpha-disk.md). In the radiation-dominated limit, $\lambda/(1+\lambda)\to1$, so $H\propto(\Omega\Sigma)^{-1}$ and

$$
\boxed{\bar\nu\propto\Omega^{-1}\Sigma^{-2}\propto r^{3/2}\Sigma^{-2}\qquad(\lambda\gg1).}
$$

For [viscous stability of an accretion disk](../../../../../../viscous-stability-of-an-accretion-disk.md), linearize the [Keplerian viscous diffusion equation](../../../../../../keplerian-viscous-diffusion-equation.md) at fixed radius: a local [mass density](../../../../../../density.md) perturbation has diffusion coefficient $3\partial_\Sigma(\bar\nu\Sigma)$. The gas branch has $\bar\nu\Sigma\propto\Sigma^{5/3}$ and a positive derivative, so it smooths perturbations. The radiation branch has $\bar\nu\Sigma\propto\Sigma^{-1}$ and a negative derivative, giving [radiation-pressure viscous instability](../../../../../../radiation-pressure-viscous-instability.md). **The gas-pressure branch is viscously stable; the radiation-pressure branch is viscously unstable in this closure.** This concerns radial mass-transport stability on wavelengths where the vertically averaged thin-disc model applies.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

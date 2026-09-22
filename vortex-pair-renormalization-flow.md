# Vortex-pair renormalization flow

↑ **Parent:** [Berezinskii–Kosterlitz–Thouless transition](berezinskii-kosterlitz-thouless-transition.md)

In the dilute-vortex description of the two-dimensional XY model, $K=\rho_s/(k_BT)$ is dimensionless stiffness and $y$ is [phase vortex](phase-vortex.md) fugacity. A [phase vortex](phase-vortex.md) has logarithmic energy $\pi\rho_s\log(L/a)$, while its placement entropy is $2k_B\log(L/a)$. Small [phase vortex](phase-vortex.md) pairs screen the logarithmic interaction, lowering the stiffness. Near $K=2/\pi$, the rescaled variables $X=2-\pi K$, $Y=4\pi y$ obey $X'=Y^2$, $Y'=XY$ to leading order. The invariant $X^2-Y^2$ leads to an essential correlation-length singularity $\xi\sim a\exp(C/\sqrt{T-T_c})$, not a finite power-law exponent.

Here $\ell=\log(r/a)$ increases toward larger observation distances, and the [vortex fugacity](vortex-fugacity.md) $y$ is a dimensionless weight per unit core, conventionally initialized as $y_0\simeq e^{-E_c/(k_BT)}$ with the microscopic measure fixed. Numerical coefficients depend on this normalization. In the displayed convention, differentiating $X=2-\pi K$ using the original flow gives

$$
X'=4\pi^4K^2y^2=\frac{(2-X)^2}{4}Y^2,
\qquad Y'=XY.
$$

Only replacing the prefactor $(2-X)^2/4$ by one near $X=0$ gives the scaled leading model. Its [first integral](first-integral.md) follows directly:

$$
\frac{d}{d\ell}(X^2-Y^2)=2XY^2-2Y(XY)=0.
$$

Thus this [first integral](first-integral.md) belongs to the stated scaled model, not exactly to the original $K,y$ equations. For $Y\geq0$, the critical [separatrix](separatrix.md) is $X=-Y$. The bound side has $X<-Y$ and flows to $Y=0$, $X<0$; the unbinding side ultimately runs to large [vortex fugacity](vortex-fugacity.md), where the dilute approximation ceases to be quantitative.

To derive the unusual [correlation length](correlation-length.md) scaling without fitting an exponent, write the invariant on a nearby unbinding trajectory as $X^2-Y^2=-c^2$. Then $X'=X^2+c^2$ and the time to cross fixed small limits $-b$ to $b$ is $2\arctan(b/c)/c\sim\pi/c$. If a physical one-parameter path crosses the [separatrix](separatrix.md) transversely, its $c^2$ is proportional to the positive [reduced temperature](reduced-temperature.md). Since distance grows as $e^\ell$, this gives $\xi\sim a\exp(b_0/\sqrt{t})$, with a nonuniversal $b_0>0$. This is the dimensionless-temperature form of the singularity above.

**Table of contents**

- [Finite-scale vortex renormalization](finite-scale-vortex-renormalization.md)

## ↑ Ancestors (7)

1. [Berezinskii–Kosterlitz–Thouless transition](berezinskii-kosterlitz-thouless-transition.md)
2. [Lower critical dimension](lower-critical-dimension.md)
3. [Critical phenomenon](critical-phenomenon-split.md)
4. [Statistical physics](statistical-physics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-69/3/b/solution.md)
- [Universal stiffness jump](universal-stiffness-jump.md)
- [Vortex fugacity](vortex-fugacity.md)

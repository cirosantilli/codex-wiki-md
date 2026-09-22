<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [gravity-capillary drop with a meridional curvature approximation](../../../../gravity-capillary-drop-with-a-meridional-curvature-approximation.md) uses the stipulated $\kappa=-h''$ for this calculation. At equilibrium the [thin-film equation](../../../../thin-film-equation.md) gives

$$
rh^3(\rho gh'-\gamma h''')=C.
$$

Regularity at $r=0$ forces $C=0$. In the wetted interior $h>0$, the equilibrium [pressure gradient](../../../../pressure-gradient.md) therefore vanishes, giving

$$
h'''-\frac{h'}{l^2}=0,\qquad
\boxed{l=\sqrt{\frac{\gamma}{\rho g}}.}
$$

This is the [capillary length](../../../../capillary-length.md). Integrating the constant-coefficient [ordinary differential equation](../../../../ordinary-differential-equation.md) gives

$$
h=C_0+C_1\cosh(r/l)+C_2\sinh(r/l).
$$

The central [boundary condition](../../../../boundary-condition.md) $h'(0)=0$ sets $C_2=0$, and contact at $r=R$ gives $C_0=-C_1\cosh(R/l)$. Write $C_1=-\alpha l$. The prescribed [contact angle](../../../../contact-angle.md) fixes

$$
h'(R)=-\alpha\sinh(R/l)=-\tan\theta_c,
\qquad
\boxed{\alpha=\frac{\tan\theta_c}{\sinh(R/l)},\quad
h(r)=\alpha l[\cosh(R/l)-\cosh(r/l)].}
$$

Here $\alpha$ is the dimensionless coefficient of this drop solution, unrelated to the hinge angle in question 1.

The axisymmetric [volume integral](../../../../volume-integral.md) is $V=2\pi\int_0^Rrh(r)\,dr$. Substituting $\xi=r/l$ gives

$$
\boxed{1=\frac{2\pi l^3\alpha}{V}\int_0^{R/l}[\cosh(R/l)-\cosh\xi]\xi\,d\xi.}
$$

For numerical evaluation, with $s=R/l$, the integral is

$$
I(s)=\frac{s^2}{2}\cosh s-s\sinh s+\cosh s-1.
$$

Together with $\alpha=\tan\theta_c/\sinh s$, this determines $R$ for fixed $V$ and $\theta_c$.

The [Bond number](../../../../bond-number.md) $R^2/l^2=\rho gR^2/\gamma$ distinguishes the dominant balances. For $R\ll l$, [surface tension](../../../../surface-tension-split.md) dominates [gravity](../../../../gravity.md) and the surface is nearly a small-slope constant-[curvature](../../../../curvature.md) cap:

$$
h(r)\approx\frac{\tan\theta_c}{2R}(R^2-r^2),\qquad
V\approx\frac{\pi\tan\theta_c}{4}R^3.
$$

For $R\gg l$, [gravity](../../../../gravity.md) flattens the interior, while [surface tension](../../../../surface-tension-split.md) bends the edge over the [capillary length](../../../../capillary-length.md). The stipulated model gives

$$
h(0)\approx l\tan\theta_c,\qquad
V\approx\pi R^2l\tan\theta_c,
$$

up to relative corrections of order $l/R$. The [contact angle](../../../../contact-angle.md) fixes the edge slope and therefore the height scale; [conservation of mass](../../../../mass-conservation.md) then fixes the lateral extent. Consistency of [lubrication theory](../../../../lubrication-theory.md) requires small slopes, in particular $\tan\theta_c\ll1$.

**The stated approximation differs from [axisymmetric free-surface curvature](../../../../axisymmetric-free-surface-curvature.md).** For an axisymmetric graph with the same sign convention, the sum of principal [curvatures](../../../../curvature.md) is

$$
\kappa=-\frac1r\frac{d}{dr}\left(\frac{rh'}{\sqrt{1+h'^2}}\right)
\approx-\left(h''+\frac{h'}r\right).
$$

The omitted $h'/r$ term is generally of the same order as $h''$. For example, $h=H(1-r^2/R^2)$ gives stipulated $\kappa=2H/R^2$ but axisymmetric small-slope $\kappa=4H/R^2$. Thus the required hyperbolic-cosine profile solves the explicitly prescribed reduced model, not the full axisymmetric capillary equilibrium. Keeping both small-slope terms instead gives

$$
h(r)=\frac{l\tan\theta_c}{I_1(R/l)}[I_0(R/l)-I_0(r/l)],
$$

where $I_0,I_1$ are [modified Bessel functions](../../../../modified-bessel-function.md). The qualitative [capillary length](../../../../capillary-length.md) and [Bond number](../../../../bond-number.md) balances remain valid.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the fluids course of the University of Oxford](../../../split.md)
5. [Fluids course of the University of Oxford](../../../../fluids-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

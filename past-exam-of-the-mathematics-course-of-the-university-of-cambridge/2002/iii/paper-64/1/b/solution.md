<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [first-order phase transition](../../../../../../first-order-phase-transition.md) has a discontinuity in a first derivative of the equilibrium [free energy](../../../../../../thermodynamic-free-energy.md), such as [entropy](../../../../../../entropy.md) or the [order parameter](../../../../../../order-parameter.md); a thermal first-order transition normally has [latent heat](../../../../../../latent-heat.md). At a [continuous phase transition](../../../../../../continuous-phase-transition.md) the [order parameter](../../../../../../order-parameter.md) goes continuously to zero and there is no [latent heat](../../../../../../latent-heat.md), although response functions and higher derivatives of the [free energy](../../../../../../thermodynamic-free-energy.md) can be singular.

For the symmetric scalar [Landau free energy](../../../../../../landau-free-energy.md) at zero conjugate field, minimize

$$
V(M)=\frac r2M^2+\frac u4M^4+\frac v6M^6,\qquad
V'(M)=M(r+uM^2+vM^4).
$$

If $u>0$, the sixth-order term is unnecessary near $r=0$. For $r>0$ the minimum is $M=0$, whereas for $r<0$ there are two symmetry-related minima with $M^2=-r/u$ to leading order. The [order parameter](../../../../../../order-parameter.md) vanishes continuously as $r\uparrow0$. The equilibrium [free-energy density](../../../../../../free-energy-density.md) changes from zero to $-r^2/(4u)$, so its first temperature derivative is continuous and its second derivative has a jump. This is the ordinary mean-field [continuous phase transition](../../../../../../continuous-phase-transition.md).

If $u<0$, keep $v>0$ for stability. A nonzero stationary [order parameter](../../../../../../order-parameter.md), with $s=M^2$, obeys $r+us+vs^2=0$. For [phase coexistence](../../../../../../phase-coexistence.md) with $M=0$ its [free energy](../../../../../../thermodynamic-free-energy.md) must also vanish. Substituting $r=-us-vs^2$ into $V$ gives

$$
V=-\frac u4s^2-\frac v3s^3.
$$

The nonzero solution of $V=0$ is therefore

$$
\boxed{M_t^2=-\frac{3u}{4v},\qquad r_t=\frac{3u^2}{16v}.}
$$

The competing minima exchange stability at positive $r_t$, with a finite jump of the [order parameter](../../../../../../order-parameter.md). This is a [first-order phase transition](../../../../../../first-order-phase-transition.md). The [metastability](../../../../../../metastability.md) region is also visible: nonzero stationary points first appear at the [spinodal](../../../../../../spinodal.md) $r=u^2/(4v)$, and the disordered local minimum loses stability at $r=0$.

For example, holding $u,v$ fixed and taking $r=a(T-T_0)$, the ordered phase has [entropy](../../../../../../entropy.md) lower than the disordered phase by $aM_t^2/2$ at coexistence. Heating through the transition absorbs [latent heat](../../../../../../latent-heat.md) per volume $T_taM_t^2/2$. More generally the temperature dependence of all coefficients contributes to this [entropy](../../../../../../entropy.md) difference. With no inversion symmetry, a cubic term can also produce a [first-order phase transition](../../../../../../first-order-phase-transition.md), as comparison of the competing minima of the [Landau free energy](../../../../../../landau-free-energy.md) shows.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

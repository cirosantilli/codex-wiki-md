<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the downward-positive displacement and the [filament bending modulus](../../../../../../filament-bending-modulus.md) $B$ and load density $w$ defined above. Two applications of [integration by parts](../../../../../../integration-by-parts.md) give the [first variation](../../../../../../first-variation.md)

$$
\delta E=\int_0^L(Bh_{xxxx}-w)\delta h\,dx
+B[h_{xx}\delta h_x-h_{xxx}\delta h]_0^L.
$$

Thus the elastic-plus-gravitational [force](../../../../../../force.md) density is $-\delta E/\delta h=-Bh_{xxxx}+w$. In [resistive-force theory](../../../../../../resistive-force-theory.md), transverse motion has drag per unit length $-\zeta_\perp h_t$. Neglecting filament and fluid inertia, instantaneous force balance gives the forced [small-slope elastohydrodynamic filament equation](../../../../../../small-slope-elastohydrodynamic-filament-equation.md)

$$
\boxed{\zeta_\perp h_t=-Bh_{xxxx}+w.}
$$

Clamping fixes position and tangent, while the free end has zero bending moment and zero transverse shear force. Therefore

$$
\boxed{h(0,t)=h_x(0,t)=0,\qquad h_{xx}(L,t)=h_{xxx}(L,t)=0.}
$$

The last two conditions also follow as natural boundary conditions from the variation, since the free-end values of $\delta h$ and $\delta h_x$ are arbitrary. Distributed weight does not add a concentrated force or moment at the tip.

At steady state, $Bh_s''''=w$. Integrating first from the free end gives $h_s'''=(w/B)(x-L)$ and $h_s''=(w/2B)(x-L)^2$. Integrating twice more with the clamp conditions gives the [uniform-load bending of a clamped filament](../../../../../../uniform-load-bending-of-a-clamped-filament.md):

$$
\boxed{h_s(x)=\frac{w}{24B}x^2(x^2-4Lx+6L^2).}
$$

In particular the free-end displacement is $\delta=h_s(L)=wL^4/(8B)$ and the total buoyancy-corrected gravitational load is $F=wL$. Thus the [tip stiffness of a uniformly loaded cantilever](../../../../../../tip-stiffness-of-a-uniformly-loaded-cantilever.md) is

$$
\boxed{F=k_{\rm eff}\delta,\qquad k_{\rm eff}=\frac{8B}{L^3}
=\frac{2\pi A a^4}{L^3}.}
$$

The last expression uses $A$ as [Young's modulus](../../../../../../young-s-modulus.md); if $A$ itself is flexural rigidity, the same result reads $k_{\rm eff}=8A/L^3$. This is [Hooke's law](../../../../../../hooke-s-law.md) for the specified loading pattern. It is not the stiffness for a point force at the tip, which would be $3B/L^3$; replacing a distributed force by its resultant does not preserve its bending moment distribution.

For [dimensional analysis](../../../../../../dimensional-analysis.md), $[A]=$ force/length squared, $[I]=$ length to the fourth power, hence $[B]=$ force times length squared. Consequently $[B/L^3]=$ force/length, as required for a spring constant. Also $[\zeta_\perp]=$ force times time/length squared makes $\zeta_\perp h_t$, $Bh_{xxxx}$ and $w$ all forces per unit length. Neither viscosity nor density enters the stiffness, although viscous drag controls the rate of approach to the steady shape. The small-slope approximation requires $wL^3/B\ll1$, since $h_s'(L)=wL^3/(6B)$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 342](../../../paper-342-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

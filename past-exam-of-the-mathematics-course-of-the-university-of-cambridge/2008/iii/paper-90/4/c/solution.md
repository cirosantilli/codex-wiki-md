<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In a homogeneous ambient fluid, $N=0$ and $R=\rho_0$ is constant. Use kinematic fluxes or, equivalently, the primitive form of the [unsteady top-hat line-plume balances](../../../../../../unsteady-top-hat-line-plume-balances.md):

$$
b_t+(bw)_z=\alpha w,\qquad
(bw)_t+(bw^2)_z=bg',\qquad
(bg')_t+(bg'w)_z=0.
$$

Here $g'=g(\rho_0-\rho)/R>0$ is the positive buoyant [reduced gravity](../../../../../../reduced-gravity-split.md). Seek a nonsteady separable [power-law ansatz](../../../../../../power-law-ansatz.md) with both time differentiation and vertical transport retained. Matching powers in the volume equation forces $b\propto z$ with no time dependence. Matching the two momentum terms then gives $w\propto z/\tau$, and the [buoyancy](../../../../../../buoyancy.md) force has $g'\propto z/\tau^2$, where $\tau=t+t_*>0$ is a shifted age. Thus write

$$
b=Bz,\qquad w=A\frac z\tau,\qquad g'=C\frac z{\tau^2}.
$$

Substitution determines the constants rather than just the exponents. The volume equation gives $2BA=\alpha A$, so for a nonzero [buoyant plume](../../../../../../buoyant-plume.md) $B=\alpha/2$. The momentum equation gives $C=-A+3A^2$, while the [buoyancy](../../../../../../buoyancy.md) equation gives $C(-2+3A)=0$. The buoyant nontrivial branch has $A=2/3$ and $C=2/3$. Consequently the [separable decaying top-hat line plume](../../../../../../separable-decaying-top-hat-line-plume.md) is

$$
\boxed{b=\frac{\alpha z}{2},\qquad
w=\frac{2z}{3\tau},\qquad
g'=\frac{2z}{3\tau^2},\qquad
\rho=R\left(1-\frac{2z}{3g\tau^2}\right).}
$$

The [Boussinesq approximation](../../../../../../boussinesq-approximation.md) requires $2z/(3g\tau^2)\ll1$. The corresponding [mass density](../../../../../../density.md)-weighted fluxes, to this order, are

$$
\boxed{Q=\frac{R\alpha z^2}{3\tau},\qquad
M=\frac{2R\alpha z^3}{9\tau^2},\qquad
F=\frac{2R\alpha z^3}{9\tau^3}.}
$$

For a direct check, $Q^2/M=R\alpha z/2$ is time independent and $FQ/M=R\alpha z^2/(3\tau^2)$. Hence $(Q^2/M)_t+Q_z=2R\alpha z/(3\tau)=R\alpha M/Q$, $Q_t+M_z=R\alpha z^2/(3\tau^2)=FQ/M$, and $(FQ/M)_t+F_z=0$. This verifies all three balances and the required width coefficient.

This nonsteady branch is not the steady, continuously supplied, constant-flux [line plume](../../../../../../line-plume.md). The latter has constant $w$ and half-width $b=\alpha z$ in the same top-hat convention. Also, the unshifted [power law](../../../../../../power-law.md) has $Q,F\to0$ as $z\to0$ and is singular at $\tau=0$. It is therefore an interior separable solution, not by itself a solution with a nonzero continuously operating point-source flux at the origin. A finite-width source boundary, a virtual origin, or a matching region is needed to connect it to physical source and initial data. For example, replacing $z$ by $z+z_*$ supplies a finite base width and time-varying positive base fluxes when $z_*>0$. No source or initial flux history is specified in the question to select that matching; the requested power-law width follows from the local balances above.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 90](../../../paper-90-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

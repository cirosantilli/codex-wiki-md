<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Seek a nonzero-buoyancy, separable [similarity solution](../../../../../../similarity-solution.md) of the [unsteady Boussinesq triangular-profile line-plume balances](../../../../../../unsteady-boussinesq-triangular-profile-line-plume-balances.md), using powers of distance and time. Let $\tau=t+t_*>0$, allowing a time origin, and initially take distance $z$ from the virtual origin. Balancing the powers in the [momentum](../../../../../../momentum.md) and buoyancy equations and the entrainment balance gives the form

$$
Q=A\frac{z^2}{\tau},\qquad M=B\frac{z^3}{\tau^2},\qquad F=C\frac{z^3}{\tau^3}.
$$

One way to recover the exponents is to let $Q\propto z^a\tau^p$ and $M\propto z^b\tau^q$. Matching the spatial powers in $\partial_t(Q^2/M)$, $Q_z$ and $M/Q$ gives $a=2,b=3$; matching the time powers gives $p=-1,q=-2$. The [momentum](../../../../../../momentum.md) equation then gives the powers of $F$. In the resulting solution, $Q^2/M$ is time-independent, so the storage term in the first equation vanishes exactly.

Direct substitution yields the coefficient equations

$$
2A=3\alpha\rho_0\frac BA,\qquad -A+3B=\frac{CA}{B},\qquad -2\frac{CA}{B}+3C=0.
$$

For a rising buoyant solution $C>0$, the last equation gives $B=2A/3$. The first then gives $A=\alpha\rho_0$, and the second gives $C=B$. The [separable decaying line-plume similarity](../../../../../../separable-decaying-line-plume-similarity.md) is therefore

$$
\boxed{Q=\alpha\rho_0\frac{z^2}{\tau},\qquad
M=\frac23\alpha\rho_0\frac{z^3}{\tau^2},\qquad
F=\frac23\alpha\rho_0\frac{z^3}{\tau^3}.}
$$

Reconstructing the physical fields confirms

$$
\boxed{W=\frac z\tau,\qquad b=\alpha z,\qquad
\frac{g(\rho_0-\rho)}{\rho_0}=\frac z{\tau^2}.}
$$

For example, $\partial_t(FQ/M)=-2\alpha\rho_0z^2/\tau^3$ and $F_z=2\alpha\rho_0z^2/\tau^3$ cancel; the [momentum](../../../../../../momentum.md) balance similarly gives $-\alpha\rho_0z^2/\tau^2+2\alpha\rho_0z^2/\tau^2=FQ/M$.

The unshifted form uses $t_*=0$ and is defined for $t>0$, with a singular zero-time limit. To give a finite solution for all $t\ge0$, choose $t_*>0$. The equations also permit replacing $z$ by $z+z_*>0$, a [plume virtual origin](../../../../../../plume-virtual-origin.md); at a finite physical source distance this family has flux histories proportional to $\tau^{-1},\tau^{-2},\tau^{-3}$. The [Boussinesq approximation](../../../../../../boussinesq-approximation.md) requires $(z+z_*)/(g\tau^2)\ll1$ in the region modelled. **This is a decaying similarity family; its time and virtual origins require source or initial data.** The PDF supplies neither, so a unique forced-startup history cannot be selected from it. In particular, the singular unshifted field should not be presented as a regular solution at $t=0$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

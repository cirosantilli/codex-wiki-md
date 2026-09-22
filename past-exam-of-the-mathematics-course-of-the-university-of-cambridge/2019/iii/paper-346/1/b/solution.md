<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The shell equation is conservative because its radial acceleration is the negative [derivative](../../../../../../derivative.md) of the specific [potential energy](../../../../../../potential-energy.md)

$$
U(r)=-\frac{GM}{r}-\frac{\Lambda r^2}{6}.
$$

Multiplying the equation of motion by $\dot r$ gives

$$
\frac{d}{dt}\left(\frac12\dot r^2-\frac{GM}{r}-\frac{\Lambda r^2}{6}\right)
=\dot r\left(\ddot r+\frac{GM}{r^2}-\frac{\Lambda r}{3}\right)=0.
$$

Hence

$$
\boxed{E=\frac12\dot r^2-\frac{GM}{r}-\frac{\Lambda r^2}{6}=\text{constant}.}
$$

This is energy per unit shell mass. The total energy of a uniform sphere requires integrating the energies of its shells.

For a sphere of physical radius $R$, the [shell theorem](../../../../../../spherical-shell-theorem.md) gives $M(r)=M(r/R)^3$ and $dM=3Mr^2\,dr/R^3$. Assemble the sphere shell by shell to obtain its [Newtonian gravitational potential energy](../../../../../../newtonian-gravitational-potential-energy.md):

$$
W_G(R)=-\int_0^R\frac{GM(r)}r\,dM
=-\frac{3GM^2}{R^6}\int_0^Rr^4\,dr
=-\frac35\frac{GM^2}{R}.
$$

The [cosmological constant](../../../../../../cosmological-constant.md) contributes a prescribed one-body potential $-\Lambda r^2/6$, rather than a pair interaction, so there is no additional factor $1/2$:

$$
W_\Lambda(R)=-\frac\Lambda6\int_0^Rr^2\,dM
=-\frac{\Lambda M}{2R^3}\int_0^Rr^4\,dr
=-\frac1{10}\Lambda MR^2.
$$

Evaluating at the [turnaround radius](../../../../../../turnaround-radius.md) gives

$$
\boxed{W_{G,\rm ta}=-\frac35\frac{GM^2}{r_{\rm ta}},\qquad
W_{\Lambda,\rm ta}=-\frac1{10}\Lambda Mr_{\rm ta}^2.}
$$

As in the question, $\Lambda$ here includes the factor $c^2$ that would multiply the geometrical [cosmological constant](../../../../../../cosmological-constant.md) in SI units.

For the final equilibrium apply the scalar [virial theorem](../../../../../../virial-theorem.md). The gravitational virial is $W_G$, whereas the [cosmological constant](../../../../../../cosmological-constant.md) force contributes

$$
\sum_\alpha\mathbf r_\alpha\cdot\mathbf F_{\Lambda,\alpha}
=\frac\Lambda3\int r^2\,dM=-2W_\Lambda.
$$

Thus, neglecting a surface-pressure term,

$$
\boxed{2T_f+W_{G,f}-2W_{\Lambda,f}=0.}
$$

At fixed $R$, a positive [cosmological constant](../../../../../../cosmological-constant.md) reduces the [kinetic energy](../../../../../../kinetic-energy.md) needed for virial equilibrium because its outward acceleration partially offsets self-gravity.

For the [uniform-sphere collapse with a cosmological constant](../../../../../../uniform-sphere-collapse-with-a-cosmological-constant.md), assume a uniform final sphere of the same mass, with no energy loss or escaping matter. Put

$$
x=\frac{r_f}{r_{\rm ta}},\qquad
A=\frac{3GM^2}{5r_{\rm ta}},\qquad
B=\frac{\Lambda Mr_{\rm ta}^2}{10}.
$$

The sphere has no bulk [kinetic energy](../../../../../../kinetic-energy.md) at turnaround, so $E_{\rm ta}=-A-B$. The final [virial theorem](../../../../../../virial-theorem.md) gives

$$
T_f=\frac{A}{2x}-Bx^2,
\qquad
E_f=T_f-\frac Ax-Bx^2=-\frac A{2x}-2Bx^2.
$$

Since $\rho_{\rm ta}=3M/(4\pi r_{\rm ta}^3)$,

$$
\frac BA=\frac{\Lambda r_{\rm ta}^3}{6GM}=\frac\eta2,
\qquad
\eta=\frac{\Lambda}{4\pi G\rho_{\rm ta}}.
$$

[Conservation of energy](../../../../../../conservation-of-energy.md) therefore gives

$$
1+\frac\eta2=\frac1{2x}+\eta x^2,
\qquad
\boxed{2\eta x^3-(2+\eta)x+1=0.}
$$

Select the collapsing branch continuous from $x=1/2$ at $\eta=0$, rather than an unrelated root of the [cubic equation](../../../../../../cubic-equation.md).

For $|\eta|\ll1$, the root lies close to $1/2$. Linearize $x^3$ there:

$$
x^3=\frac18+\frac34\left(x-\frac12\right)
+O\!\left((x-\tfrac12)^2\right)
=\frac34x-\frac14+O\!\left((x-\tfrac12)^2\right).
$$

Substitution into the [cubic equation](../../../../../../cubic-equation.md) gives $(\eta/2-2)x+1-\eta/2\simeq0$, whence

$$
\boxed{\frac{r_f}{r_{\rm ta}}\simeq\frac{1-\eta/2}{2-\eta/2}
=\frac12-\frac\eta8+O(\eta^2).}
$$

The rational expression is an approximation, not an exact solution of the [cubic equation](../../../../../../cubic-equation.md). In fact both it and the exact collapsing root agree through order $\eta^2$; their first difference is of order $\eta^3$.

With zero [cosmological constant](../../../../../../cosmological-constant.md), [spherical collapse](../../../../../../spherical-collapse-model.md) gives $r_f=r_{\rm ta}/2$. For small positive $\Lambda$, the same sphere with the same [turnaround radius](../../../../../../turnaround-radius.md) reaches a smaller final radius. This does not mean that repulsion promotes collapse: as the sphere contracts, $W_\Lambda$ becomes less negative, so some released gravitational binding energy pays the energetic cost of moving inward against the repulsive force. Combined with the modified [virial theorem](../../../../../../virial-theorem.md), energy conservation requires a more compact endpoint. Positive $\Lambda$ can prevent turnaround altogether; an inward acceleration at $r_{\rm ta}$ requires

$$
-\frac{GM}{r_{\rm ta}^2}+\frac\Lambda3r_{\rm ta}<0,
\qquad\boxed{\eta<1.}
$$

The perturbative radius formula applies well inside this limit, for spheres that actually turn around. A small negative [cosmological constant](../../../../../../cosmological-constant.md) instead gives $r_f/r_{\rm ta}>1/2$ at fixed turnaround data.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 346](../../../paper-346-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

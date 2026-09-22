<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $\mathcal G$ be the outward [viscous torque in an accretion disk](../../../../../../viscous-torque-in-an-accretion-disk.md). For a declining [angular velocity](../../../../../../angular-velocity.md), the vertically integrated viscous shear stress gives

$$
\mathcal G=-2\pi\nu\Sigma r^3\Omega'(r)>0.
$$

In a steady [accretion disk](../../../../../../accretion-disk.md) without radiated [angular momentum](../../../../../../angular-momentum.md), the net inward [angular-momentum flux](../../../../../../angular-momentum-flux.md) $Fh-\mathcal G$ is constant and equals the swallowed flux $Fh_0$. Thus [conservation of angular momentum](../../../../../../conservation-of-angular-momentum.md) gives $F(h-h_0)=\mathcal G$. Substituting $F=2\pi r\Sigma u$ cancels the [surface density](../../../../../../surface-density-of-a-disk.md) and proves

$$
\boxed{u=\frac{\nu r^2[-\Omega'(r)]}{h-h_0}.}
$$

This uses the stipulated phenomenological viscous shear law; it does not replace it by a different fully relativistic stress prescription.

For the orbital calculation let a dot denote a derivative with respect to [proper time](../../../../../../proper-time.md). Substituting the geodesic energy and [specific angular momentum](../../../../../../specific-angular-momentum.md) first integrals into the timelike normalization in [Schwarzschild spacetime](../../../../../../schwarzschild-spacetime.md) gives

$$
\dot r^2=\frac{\epsilon^2}{c^2}-\left(1-\frac{2m}{r}\right)\left(c^2+\frac{h^2}{r^2}\right).
$$

Differentiate with $h$ and $\epsilon$ constant along the [geodesic](../../../../../../geodesic.md). Where $\dot r\ne0$, division by $2\dot r$ gives

$$
\ddot r=-\frac12\frac d{dr}\left[\left(1-\frac{2m}{r}\right)\left(c^2+\frac{h^2}{r^2}\right)\right]
=\boxed{-\frac{mc^2}{r^2}+\frac{h^2}{r^3}\left(1-\frac{3m}{r}\right).}
$$

This equation also holds at turning points and on [circular orbits](../../../../../../circular-orbit.md). To justify that without dividing by zero, put $A=1-2m/r$ in the equatorial geodesic [Lagrangian](../../../../../../lagrangian.md) $L=(Ac^2\dot t^2-A^{-1}\dot r^2-r^2\dot\phi^2)/2$. Its radial [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md) is $\ddot r=(A'/2A)\dot r^2-AA'c^2\dot t^2/2+Ar\dot\phi^2$. Substitution of the timelike normalization cancels the $\dot r^2$ terms and yields $\ddot r=-A'c^2/2+(A/r-A'/2)h^2/r^2$, exactly the displayed radial equation, including when $\dot r=0$.

A [circular orbit](../../../../../../circular-orbit.md) requires $\ddot r=\dot r=0$. Therefore

$$
h^2=\frac{mc^2r^2}{r-3m},\qquad
\boxed{h(r)=rc\sqrt{\frac m{r-3m}}},\qquad r>3m,
$$

choosing the positive sense of rotation. Differentiating the square is simpler than differentiating $h$:

$$
\frac d{dr}h^2=mc^2\frac{r(r-6m)}{(r-3m)^2}.
$$

It is negative for $3m<r<6m$ and positive for $r>6m$, so the global minimum over timelike [circular orbits](../../../../../../circular-orbit.md) is

$$
\boxed{r_0=6m,\qquad h_0=\sqrt{12}\,mc.}
$$

As a stability check, the second radial derivative of $W=(1-2m/r)(c^2+h^2/r^2)$ at a [circular orbit](../../../../../../circular-orbit.md), holding $h$ fixed for the perturbation, is $W''=2mc^2(r-6m)/[r^3(r-3m)]$. Thus the exterior branch is stable, and $6m$ is the [innermost stable circular orbit](../../../../../../innermost-stable-circular-orbit.md). It is the natural matching radius for the idealized [zero-torque inner boundary condition](../../../../../../zero-torque-inner-boundary-condition.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

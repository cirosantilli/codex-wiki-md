<h1 id="section-c/c10/solution">Solution</h1>

↑ **Parent:** [C10](../c10.md)

A [normal mode](../../../../../normal-mode.md) is a motion in which all [displacement](../../../../../displacement.md) coordinates oscillate at one [angular frequency](../../../../../angular-frequency.md) with fixed [amplitude](../../../../../wave-amplitude.md) ratios. For small conservative oscillations, the symmetric stiffness and [mass](../../../../../mass.md) matrices give the [generalized eigenvalue problem for small oscillations](../../../../../generalized-eigenvalue-problem-for-small-oscillations.md), $\mathsf K\mathbf u=\omega^2\mathsf M\mathbf u$. For positive [mass](../../../../../mass.md) and a stable equilibrium, its mass-orthogonal [eigenvectors](../../../../../eigenvector.md) span the motion. A [superposition](../../../../../superposition-principle.md) of these modes, with phases and [amplitudes](../../../../../wave-amplitude.md) fixed by initial [displacements](../../../../../displacement.md) and [velocities](../../../../../velocity.md), gives the general solution; different modes need not share a phase.

Use upward end [displacements](../../../../../displacement.md). The [spring](../../../../../spring.md) compressions are $x_0-x_1$ and $x_0-x_2$, while the beam's centre rises by $q=(x_1+x_2)/2$. The [potential energy](../../../../../potential-energy.md) is

$$
V=\frac k2[(x_0-x_1)^2+(x_0-x_2)^2]+\frac{mg}{2}(x_1+x_2).
$$

Static [force balance](../../../../../force-balance.md) gives $2kx_0=mg$, cancelling the linear terms and leaving

$$
\boxed{V=\tfrac12k(x_1^2+x_2^2)+kx_0^2.}
$$

For a uniform beam, its central [moment of inertia](../../../../../moment-of-inertia.md) in the vertical plane is $ml^2/12$. To first order in the tilt, $\theta=(x_2-x_1)/l$. Its translational and rotational [kinetic energies](../../../../../kinetic-energy.md) are

$$
T=\frac m8(\dot x_1+\dot x_2)^2+\frac m{24}(\dot x_2-\dot x_1)^2
=\frac m6(\dot x_1^2+\dot x_1\dot x_2+\dot x_2^2).
$$

Thus $\mathsf M=(m/6)\begin{pmatrix}2&1\\1&2\end{pmatrix}$ and $\mathsf K=k\mathsf1$. The [normal modes of a rigid beam on two end springs](../../../../../normal-modes-of-a-rigid-beam-on-two-end-springs.md) have [eigenvectors](../../../../../eigenvector.md)

$$
\boxed{\mathbf u_s=(1,1),\quad\omega_s=\sqrt{2k/m};\qquad
\mathbf u_a=(1,-1),\quad\omega_a=\sqrt{6k/m}.}
$$

The first translates without tilt; the second rocks about a stationary centre. Ordinary [frequencies](../../../../../frequency.md) are $\omega_s/(2\pi)$ and $\omega_a/(2\pi)$.

Assume the system had settled before the end load leaves, and put that load at end 1. Its extra static [spring](../../../../../spring.md) load is $Mg$ at that end and zero at the other. Therefore $x_1(0)=-Mg/k$, $x_2(0)=0$, and both initial [velocities](../../../../../velocity.md) vanish because no [impulse](../../../../../impulse.md) is imparted. Decomposing into the two [normal modes](../../../../../normal-mode.md) gives

$$
x_1(t)=-\frac{Mg}{2k}(\cos\omega_st+\cos\omega_at),\qquad
x_2(t)=-\frac{Mg}{2k}(\cos\omega_st-\cos\omega_at).
$$

Only the symmetric mode contributes to the centre position:

$$
\boxed{z_{\rm CM}(t)-z_{\rm eq}=-\frac{Mg}{2k}\cos\left(\sqrt{\frac{2k}{m}}\,t\right).}
$$

The datum $z_{\rm eq}$ is the unloaded beam's equilibrium height; no absolute height is supplied. The rocking mode is present even though it cancels out of this coordinate. These results use small tilt, $Mg/(kl)\ll1$, ideal light vertical [springs](../../../../../spring.md) and negligible [damping](../../../../../damping.md).

## ↑ Ancestors (14)

1. [C10](../c10.md)
2. [Section C](../../section-c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)

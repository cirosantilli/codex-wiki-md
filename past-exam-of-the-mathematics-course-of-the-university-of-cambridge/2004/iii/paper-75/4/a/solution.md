<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $V=4\pi b^3/3$ and $B=Vg(\rho_0-\rho)/\rho_{\rm ref}$. The four balances describe, respectively, [fluid entrainment](../../../../../../fluid-entrainment.md) through the spherical surface at normal speed $\alpha u$, the increase of vertical [momentum](../../../../../../momentum.md) due to [buoyancy](../../../../../../buoyancy.md), conservation of total buoyancy in a uniform ambient, and motion of the thermal centre. Entrained ambient fluid initially has no vertical [momentum](../../../../../../momentum.md), so the momentum equation includes the inertia needed to accelerate it. This model neglects [added mass](../../../../../../added-mass.md) and drag; these effects would alter the numerical similarity coefficients.

With $|\rho-\rho_0|\ll\rho_0$, the [Boussinesq approximation](../../../../../../boussinesq-approximation.md) replaces inertial density by $\rho_0$ while retaining the density difference in [buoyancy](../../../../../../buoyancy.md). Take $\rho_{\rm ref}=\rho_0$ to this accuracy. Then

$$
\dot b=\alpha u,\qquad \frac{d(Vu)}{dt}=B_0,\qquad B=B_0,\qquad \dot z=u.
$$

For a point source, $b(0)=z(0)=0$ and the initial integrated impulse is zero. Therefore $b=\alpha z$ and $Vu=B_0t$. Integrating $b^3\dot b=3\alpha B_0t/(4\pi)$ yields

$$
\boxed{b(t)=\left(\frac{3\alpha B_0}{2\pi}\right)^{1/4}t^{1/2},\qquad z(t)=\frac{b(t)}\alpha,\qquad u(t)=\frac{b(t)}{2\alpha t}}.
$$

The [mass density](../../../../../../density.md) follows from conserved buoyancy:

$$
\boxed{\rho(t)=\rho_0-\frac{3\rho_{\rm ref}B_0}{4\pi g\,b(t)^3}}.
$$

Thus the radius and rise height grow as $t^{1/2}$, the rise speed decays as $t^{-1/2}$, and the density deficit decays as $t^{-3/2}$. In height coordinates, put $K=4\pi\alpha^3/3$ and $C=\sqrt{B_0/(2K)}$; then $V=Kz^3$ and $u=C/z$.

If a reference density different from the inertial ambient density is retained, $d(Vu)/dt=(\rho_{\rm ref}/\rho_0)B_0$: replace $B_0$ in the kinematic formulas by $(\rho_{\rm ref}/\rho_0)B_0$, while retaining the original $B_0$ in the density-deficit formula. This keeps reference-density normalization separate from the physical acceleration.

The [point-source spherical thermal similarity](../../../../../../point-source-spherical-thermal-similarity.md) is singular at $t=0$ and cannot satisfy the small-density-difference condition arbitrarily close to its formal origin. A finite-radius, zero-impulse regularization has $b=b_s+\alpha z$ and $b^4=b_s^4+3\alpha B_0t^2/(2\pi)$, with $u=B_0t/V$. This displays the required initial data rather than attributing the singularity to a physical infinite initial speed.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

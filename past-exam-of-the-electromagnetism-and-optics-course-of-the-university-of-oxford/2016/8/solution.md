<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

Let $\rho_q=3q/(4\pi a^3)$ be the uniform [charge density](../../../charge-density.md) and take $\boldsymbol\omega=\omega\widehat{\mathbf z}$. Rigid rotation produces [current density](../../../current-density.md) $\mathbf J=\rho_q\boldsymbol\omega\times\mathbf r$. The [magnetic dipole moment](../../../magnetic-dipole-moment.md) is

$$
\mathbf m_s=\frac12\int\mathbf r\times\mathbf J\,d^3r
=\frac{\rho_q}{2}\int\left[r^2\boldsymbol\omega-\mathbf r(\mathbf r\cdot\boldsymbol\omega)\right]d^3r.
$$

[Spherical symmetry](../../../spherical-symmetry.md) gives $\int r_i r_j\,d^3r=\delta_{ij}\int r^2d^3r/3$, while $\int r^2d^3r=4\pi a^5/5$. Therefore

$$
\boxed{\mathbf m_s=\frac{qa^2}{5}\boldsymbol\omega.}
$$

It is parallel to the [angular velocity](../../../angular-velocity.md) for positive $q$ and antiparallel for negative $q$. The fully signed magnitude statement is $|\mathbf m_s|=|q|\,|\omega|a^2/5$; the printed magnitude assumes positive $q$ and positive angular speed.

[Axisymmetry](../../../axisymmetric-vector-field.md) permits a purely azimuthal [magnetic vector potential](../../../magnetic-vector-potential.md), $\mathbf A=f(r)\sin\theta\,\widehat{\boldsymbol\varphi}$, with $A_r=A_\theta=0$. For the source's [associated Legendre function](../../../associated-legendre-function.md) convention, $P_1^1(\cos\theta)=+\sin\theta$, since its definition omits the Condon–Shortley phase. The given differential operator reduces to

$$
\widehat F[f(r)\sin\theta]=\left(f''+\frac2r f'-\frac{2f}{r^2}\right)\sin\theta.
$$

Inside the sphere, $J_\varphi=\rho_q\omega r\sin\theta$. Since the radial operator maps $r^3$ to $10r$, the particular coefficient is $\alpha_0=-\mu_0\rho_q\omega/10$. Regularity at the origin and decay at infinity give

$$
f_{\rm in}=Ar-\frac{\mu_0\rho_q\omega}{10}r^3,\qquad
f_{\rm out}=\frac C{r^2}.
$$

There is no surface sheet [electric current](../../../electric-current.md), so both normal and tangential [magnetic field](../../../magnetic-field-split.md) components are continuous at $r=a$. Using

$$
B_r=\frac{2f(r)}r\cos\theta,\qquad
B_\theta=-\frac{f(r)+rf'(r)}r\sin\theta,
$$

this is equivalent to continuity of $f$ and $f'$. The two equations give $A=\mu_0\rho_q\omega a^2/6$ and $C=\mu_0\rho_q\omega a^5/15$. Thus

$$
\boxed{\mathbf A_{\rm in}=\frac{\mu_0\rho_q}{30}(5a^2-3r^2)(\boldsymbol\omega\times\mathbf r),\quad r<a,}
$$



$$
\boxed{\mathbf A_{\rm out}=\frac{\mu_0}{4\pi}\frac{\mathbf m_s\times\mathbf r}{r^3},\quad r>a.}
$$

In the homogeneous expansion, $\alpha_1=A$, $\beta_1=C$ in their respective interior and exterior regions; all higher angular orders vanish. Indeed, matching the regular $r^\ell$ and decaying $r^{-\ell-1}$ terms with zero source at $\ell>1$ forces both coefficients to zero. The outside [magnetic field](../../../magnetic-field-split.md) is exactly the [magnetic dipole field](../../../magnetic-dipole-field.md) of $\mathbf m_s$, not merely its leading far-field approximation. For a positive moment along $z$, $A_\varphi=\mu_0m_s\sin\theta/(4\pi r^2)$, which is the printed cross-product magnitude expression.

For the [flux coupling of a rotating charged sphere to a circular loop](../../../flux-coupling-of-a-rotating-charged-sphere-to-a-circular-loop.md), take a loop of radius $b>a$ in the equatorial plane and use [Stokes theorem](../../../stokes-theorem.md) on the regular full [vector potential](../../../vector-potential.md), evaluated around the rim. Its linked [magnetic flux](../../../magnetic-flux.md) is

$$
\Phi_b=\oint\mathbf A\cdot d\boldsymbol\ell
=2\pi b\frac{\mu_0m_s}{4\pi b^2}=\frac{\mu_0m_s}{2b}.
$$

With $m_s=\pi a^2I_0$, the [mutual inductance](../../../mutual-inductance.md) defined using this effective [electric current](../../../electric-current.md) is

$$
\boxed{M=\frac{\Phi_b}{I_0}=\frac{\mu_0\pi a^2}{2b}.}
$$

Integrating an ideal [magnetic dipole field](../../../magnetic-dipole-field.md) through the entire disk would incorrectly use its singular expression inside the actual sphere; the rim calculation avoids that error.

For the prescribed time dependence, the quasistatic [Faraday's law of induction](../../../faraday-s-law-of-induction.md) result and the purely resistive loop approximation give

$$
\boxed{I_b(t)=-\frac1R\frac{d\Phi_b}{dt}=-\frac{\mu_0qa^2\omega_0\nu}{10bR}\cos(\nu t).}
$$

Positive loop [electric current](../../../electric-current.md) is defined to produce a positive $z$ [magnetic dipole moment](../../../magnetic-dipole-moment.md), so the minus sign is [Lenz's law](../../../lenz-s-law.md). This assumes negligible retardation and $\nu L_b\ll R$, where $L_b$ is the loop's [self-inductance](../../../self-inductance.md). If that is not negligible, the governing equation is instead $L_b\dot I_b+RI_b=-\dot\Phi_b$; $R$ alone is insufficient for the exact dynamic response.

## ↑ Ancestors (11)

1. [8](../8.md)
2. [2016](../../2016-split.md)
3. [Past exam of the electromagnetism and optics course of the University of Oxford](../../split.md)
4. [Electromagnetism and optics course of the University of Oxford](../../../electromagnetism-and-optics-course-of-the-university-of-oxford.md)
5. [Year 2 of the physics course of the University of Oxford](../../../year-2-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)

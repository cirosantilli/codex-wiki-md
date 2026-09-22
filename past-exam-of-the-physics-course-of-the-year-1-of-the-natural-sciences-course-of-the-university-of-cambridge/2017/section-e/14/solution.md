<h1 id="section-e/14/solution">Solution</h1>

↑ **Parent:** [14](../14.md)

In [electrostatics](../../../../electrostatics-split.md), [Gauss's law](../../../../gauss-s-law.md) is

$$
\boxed{\oint_{\partial\Omega}\mathbf E\cdot d\mathbf A=\frac{Q_{\mathrm{enc}}}{\epsilon_0},\qquad \boldsymbol\nabla\cdot\mathbf E=\frac\rho{\epsilon_0}.}
$$

The surface normal points outward. [Spherical symmetry](../../../../spherical-symmetry.md) makes the field radial and constant in magnitude on a concentric [Gaussian](../../../../normal-distribution.md) surface.

For a uniformly charged sphere, enclosed charge is $4\pi\rho_0r^3/3$ inside and $Q=4\pi\rho_0R^3/3$ outside. Thus the radial field is

$$
\boxed{E_r(r)=\begin{cases}\displaystyle\frac{\rho_0r}{3\epsilon_0},&0\leq r\leq R,\\[4pt]\displaystyle\frac{\rho_0R^3}{3\epsilon_0r^2},&r\geq R.\end{cases}}
$$

Set potential zero at infinity. Outside, $V=Q/(4\pi\epsilon_0r)$. Inside, integrate $dV/dr=-E_r$ from the known boundary value, obtaining

$$
\boxed{V(r)=\begin{cases}\displaystyle\frac{\rho_0}{6\epsilon_0}(3R^2-r^2),&r\leq R,\\[4pt]\displaystyle\frac{\rho_0R^3}{3\epsilon_0r},&r\geq R.\end{cases}}
$$

The field rises linearly from zero to its maximum at $R$, then falls as $r^{-2}$. The potential falls quadratically from $\rho_0R^2/(2\epsilon_0)$ to its surface value and then as $r^{-1}$. Both are continuous at the surface; there is no separate sheet of surface charge.

<a id="section-e/14/image-radial-field-and-potential-of-a-uniformly-charged-solid-sphere"></a>
![](../../../../past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2017-uniform-sphere.png)

**[Figure 5](#section-e/14/image-radial-field-and-potential-of-a-uniformly-charged-solid-sphere). Radial field and potential of a uniformly charged solid sphere**.

For the [electric field of a hydrogen ground-state electron cloud](../../../../electric-field-of-a-hydrogen-ground-state-electron-cloud.md), its enclosed charge is

$$
Q_e(r)=4\pi\int_0^r s^2\rho(s)\,ds=-\frac{4e}{a_0^3}\int_0^r s^2e^{-2s/a_0}\,ds.
$$

Writing $u=2s/a_0$ and using $\int u^2e^{-u}du=-e^{-u}(u^2+2u+2)$ gives

$$
Q_e(r)=-e\left[1-e^{-2r/a_0}\left(1+\frac{2r}{a_0}+\frac{2r^2}{a_0^2}\right)\right].
$$

The total electron-cloud charge tends to $-e$, as required. Dividing by $4\pi\epsilon_0r^2$ yields

$$
\boxed{E_{e,r}(r)=\frac e{4\pi\epsilon_0}\left[\frac{e^{-2r/a_0}-1}{r^2}+\frac{2e^{-2r/a_0}}{a_0r}+\frac{2e^{-2r/a_0}}{a_0^2}\right].}
$$

The expression is negative and therefore points inward. Its apparently singular terms cancel at small radius, leaving $E_{e,r}\simeq-er/(3\pi\epsilon_0a_0^3)$.

A distant external charge polarizes the neutral atom. Its [electric field](../../../../electric-field-split.md) displaces the positive and negative charge distributions relative to one another, giving an induced dipole $\mathbf p=\alpha\mathbf E_{\mathrm{ext}}$ with static [electric polarizability](../../../../electric-polarizability.md) $\alpha>0$. The field is stronger on the nearer side, so the opposite-charge attraction exceeds the like-charge repulsion. This is [charge-induced dipole attraction](../../../../charge-induced-dipole-attraction.md), not a net monopole charge on the atom.

Quantitatively, for external charge $Q=\pm e$ at separation $r$, the [polarization](../../../../polarization-waves.md) [energy](../../../../energy-split.md) is $U=-\alpha E_{\mathrm{ext}}^2/2$, hence

$$
\boxed{U(r)=-\frac{\alpha Q^2}{2(4\pi\epsilon_0)^2r^4},\qquad F_r=-\frac{dU}{dr}=-\frac{2\alpha Q^2}{(4\pi\epsilon_0)^2r^5}.}
$$

Here negative $F_r$ means decreasing separation. Reversing the external charge reverses the induced dipole but leaves this leading long-range [force](../../../../force-split.md) attractive and of the same magnitude. The factor one half accounts for the [energy](../../../../energy-split.md) cost of inducing the dipole.

The supplied charge density describes the unperturbed atom. Adding its electron field to the nucleus field leaves $E_{\mathrm{atom}}=e e^{-2r/a_0}(r^{-2}+2/(a_0r)+2/a_0^2)/(4\pi\epsilon_0)$, an exponentially small residual because the cloud has an infinite tail. A completely frozen density would give only that tiny sign-dependent [force](../../../../force-split.md). Allowing [polarization](../../../../polarization-waves.md) is essential to obtain the dominant attractive power-law [force](../../../../force-split.md) for either sign of external charge when $r\gg a_0$.

## ↑ Ancestors (12)

1. [14](../14.md)
2. [Section E](../../section-e.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Physics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

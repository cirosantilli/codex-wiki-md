<h1 id="38c/solution">Solution</h1>

↑ **Parent:** [38C](../38c.md)

For a plane acoustic wave propagating along $\widehat{\mathbf k}$, the linear momentum equation and dispersion $\omega=c_0k$ give $\widetilde p=\rho_0c_0u_\parallel$ and $\mathbf u=u_\parallel\widehat{\mathbf k}$. Therefore the instantaneous acoustic intensity is

$$
\boxed{\widetilde p\,\mathbf u=\rho_0c_0|\mathbf u|^2\widehat{\mathbf k}.}
$$

For harmonic complex amplitudes the time average instead has the factor one half, $\langle\mathbf I\rangle=\tfrac12\rho_0c_0|\widehat{\mathbf u}|^2\widehat{\mathbf k}$.

For a radial velocity potential, set $v=r\phi$. The spherical wave equation reduces to $v_{tt}=c_0^2v_{rr}$, so

$$
\boxed{\phi(r,t)=\frac{F(t-r/c_0)+G(t+r/c_0)}r.}
$$

No incoming radiation from infinity means $G=0$. Linearizing the moving-surface condition at $r=a$ gives $\phi_r(a,t)=i\omega a\epsilon e^{i\omega t}$, with real parts understood. Write the outgoing solution as $\phi=A e^{i\omega(t-(r-a)/c_0)}/r$. Its radial derivative at $a$ is $-A(1+i\omega a/c_0)e^{i\omega t}/a^2$. Therefore the [outgoing acoustic field of a pulsating sphere](../../../../../outgoing-acoustic-field-of-a-pulsating-sphere.md) is

$$
\boxed{\phi(r,t)=\operatorname{Re}\left\{-\frac{i\omega a^3\epsilon}{1+i\omega a/c_0}
\frac{e^{i\omega(t-(r-a)/c_0)}}r\right\}.}
$$

In the far field the velocity amplitude has magnitude $(\omega/c_0)|A|/r$. Multiply its average plane-wave intensity by the spherical area to obtain the [mean acoustic power of a pulsating sphere](../../../../../mean-acoustic-power-of-a-pulsating-sphere.md):

$$
\boxed{\langle P\rangle=\frac{2\pi\rho_0\omega^2}{c_0}|A|^2
=\frac{2\pi\rho_0\epsilon^2a^6\omega^4}{c_0[1+(\omega a/c_0)^2]}.}
$$

This is positive outward radiated power, evaluated to leading quadratic order in the small real displacement amplitude.

## ↑ Ancestors (10)

1. [38C](../38c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Multiply the perturbation PV equation by $q'/\beta$ and take an $x$ average. Periodicity makes averages of $x$ derivatives vanish, while integration by parts gives

$$
\overline{\psi_xq'}
=\partial_y(-\overline{u'v'})
+\partial_z\left(\frac{f_0^2}{N^2}\overline{\psi_x'\psi_z'}\right).
$$

Using $\rho'=-f_0\rho_0\psi_z'/g$ proves the [quasi-geostrophic wave-activity conservation law](../../../../../quasi-geostrophic-wave-activity-conservation-law.md)

$$
\boxed{A_t+\nabla\cdot\mathbf F=\frac{\overline{Q'q'}}\beta,\quad
A=\frac{\overline{q'^2}}{2\beta},\quad
\mathbf F=\left(0,-\overline{u'v'},-\frac{gf_0}{\rho_0N^2}\overline{v'\rho'}\right).}
$$

$A_t$ is local wave-activity storage, $\nabla\cdot\mathbf F$ is propagation and mean-flow forcing, and $\overline{Q'q'}/\beta$ creates or destroys wave activity. A steady unforced wave has both $A_t=0$ and $Q'=0$, hence $\nabla\cdot\mathbf F=0$ and exerts no mean force.

For $K^2=k^2+l^2$, substitution of $\widehat\psi(z)e^{ikx}\sin ly$ gives

$$
\boxed{
\frac{f_0^2}{N^2}\widehat\psi''-K^2\widehat\psi+\frac\beta U\widehat\psi
=\frac{i\alpha}{kU}\frac{f_0^2}{N^2}\widehat\psi''.}
$$

Write $(1-i\alpha/(kU))^{-1/2}=\gamma_r+i\gamma_i$, where both parts are positive. If $D=\beta/U-K^2>0$, define $M=N\sqrt D/f_0$; the decaying propagating solution is

$$
\widehat\psi=Ae^{iM(\gamma_r+i\gamma_i)z}.
$$

If $D<0$, define $M=N\sqrt{-D}/f_0$; the decaying evanescent solution is

$$
\widehat\psi=Ae^{-M(\gamma_r+i\gamma_i)z}.
$$

The boundary condition fixes $A$ from $\widehat\psi'(0)=C\widehat h$. Thermal damping therefore selects decay for either sign of $D$, producing a [thermally damped quasi-geostrophic mountain wave](../../../../../thermally-damped-quasi-geostrophic-mountain-wave.md).

Since $u'=-\psi_y'$ and $v'=\psi_x'$, quadrature in $x$ gives $\boxed{F^{(y)}=0}$. Also

$$
F^{(z)}=\frac{f_0^2}{2N^2}\operatorname{Re}(ik\widehat\psi\widehat\psi'^*).
$$

Consequently

$$
\boxed{F^{(z)}=\frac{f_0^2kM\gamma_r}{2N^2}|\widehat\psi|^2>0\quad(D>0),}
$$



$$
\boxed{F^{(z)}=-\frac{f_0^2kM\gamma_i}{2N^2}|\widehat\psi|^2<0\quad(D<0).}
$$

Both fluxes tend to zero aloft. Their vertical divergence is respectively westward and eastward wave force; the equal and opposite integrated force is exerted by the flow on the lower topography. Damping thus permits topographic drag even for the evanescent regime and reverses its sign across the stationary-wave threshold.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 333](../../paper-333-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

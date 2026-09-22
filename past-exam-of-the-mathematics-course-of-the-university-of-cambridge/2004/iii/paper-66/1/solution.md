<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

**The separated disk modes.** Away from the plane of a [razor-thin disk](../../../../../razor-thin-disk-approximation.md), there is no volume source, so the [Newtonian gravitational potential](../../../../../newtonian-gravitational-potential.md) obeys the [Laplace equation in cylindrical coordinates](../../../../../laplace-equation-in-cylindrical-coordinates.md). [Separation of variables](../../../../../separation-of-variables.md) gives

$$
\frac{(RJ')'}{RJ}=-\frac{Z''}{Z}=-k^2,\qquad J''+\frac1RJ'+k^2J=0,\qquad Z''-k^2Z=0.
$$

Here $k>0$ is a radial [wavenumber](../../../../../wavenumber.md), with units of inverse length. Regularity on the axis selects the [Bessel function of the first kind](../../../../../bessel-function-of-the-first-kind.md) $J_0(kR)$ rather than the singular second solution. Decay away from the disk, continuity across it and reflection symmetry select $Z=e^{-k|z|}$. These conditions apply to each nonzero-wavenumber mode; a uniform sheet is a separate zero-mode problem.

Integrate the [Poisson equation for Newtonian gravity](../../../../../poisson-equation-for-newtonian-gravity.md) across the disk to obtain the jump condition

$$
\Phi_z(R,0^+)-\Phi_z(R,0^-)=4\pi G\Sigma(R).
$$

For the unit-amplitude separated mode, the jump is $-2kJ_0(kR)$. Thus

$$
\boxed{\Phi_k=e^{-k|z|}J_0(kR),\qquad \Sigma_k=-\frac{k}{2\pi G}J_0(kR).}
$$

An individual basis density is signed; positive physical [surface densities](../../../../../surface-density-of-a-disk.md) are built by superposition.

**An arbitrary axisymmetric surface density.** Define its order-zero [Hankel transform](../../../../../hankel-transform.md) by

$$
\widehat\Sigma(k)=\int_0^\infty\Sigma(R')J_0(kR')R'\,dR',\qquad \Sigma(R)=\int_0^\infty\widehat\Sigma(k)J_0(kR)k\,dk.
$$

Matching the coefficients of the mode densities gives the [Hankel representation of thin-disk gravity](../../../../../hankel-representation-of-thin-disk-gravity.md),

$$
\boxed{\Phi(R,z)=-2\pi G\int_0^\infty\widehat\Sigma(k)J_0(kR)e^{-k|z|}\,dk.}
$$

The [boundary conditions](../../../../../boundary-condition.md) exclude added external fields. For sufficiently decaying [surface density](../../../../../surface-density-of-a-disk.md), this is the isolated-disk potential; for infinite scale-free disks, only potential differences or regularized forces need be finite.

**The Mestel disk.** Put $C=\Sigma_0R_0$. The [Bessel function](../../../../../bessel-function.md) integral $\int_0^\infty J_0(kR')\,dR'=1/k$, understood with a decaying regulator, gives $\widehat\Sigma=C/k$. Differentiate the potential before removing the regulator and use $J_0'=-J_1$:

$$
\Phi_R(R,0)=2\pi GC\int_0^\infty J_1(kR)\,dk=\frac{2\pi GC}{R}.
$$

The last integral is $1/R$, since $\int_0^\infty J_1(u)\,du=[-J_0(u)]_0^\infty=1$. Therefore the [circular speed](../../../../../circular-speed.md) and enclosed [mass](../../../../../mass.md) are

$$
\boxed{v_c^2=R\Phi_R=2\pi G\Sigma_0R_0=:v_0^2,\qquad M(R)=2\pi\int_0^R\Sigma(R')R'\,dR'=2\pi\Sigma_0R_0R.}
$$

Consequently $v_c^2=GM(R)/R$. This equality follows from the specific [Mestel disk](../../../../../mestel-disk.md) calculation; the spherical shell theorem cannot be applied to general disks. Its total [mass](../../../../../mass.md) and absolute potential referenced to infinity diverge. A convenient finite midplane reference is $\Phi(R,0)=v_0^2\log(R/R_0)$.

**The rotating distribution function.** Use specific [energy](../../../../../energy.md) $E=(v_R^2+v_\phi^2)/2+\Phi$ and $L_z=Rv_\phi$. For the printed positive exponential, take $\varepsilon=-E$ and $s:=\sigma>0$; $s$ has units of squared velocity. If instead $\varepsilon$ means ordinary total energy and $\sigma>0$, the velocity integral diverges, so that literal convention cannot define the requested [galactic distribution function](../../../../../galactic-distribution-function.md). Equivalently one can retain ordinary energy and choose the printed $\sigma$ negative.

With the binding-energy convention, write the amplitude as $A$ to distinguish it from the function:

$$
f=A(Rv_\phi)^q\exp\!\left[-\frac{v_R^2+v_\phi^2}{2s}\right](R/R_0)^{-v_0^2/s},\qquad v_\phi>0.
$$

Integration over both radial velocities and positive azimuthal velocities gives

$$
\begin{aligned}
\Sigma(R)&=A R^q(R/R_0)^{-v_0^2/s}\sqrt{2\pi s}\,\frac{(2s)^{(q+1)/2}}{2}\Gamma\!\left(\frac{q+1}{2}\right)\\
&=A R^q(R/R_0)^{-v_0^2/s}\sqrt\pi\,2^{q/2}s^{(q+2)/2}\Gamma\!\left(\frac{q+1}{2}\right).
\end{aligned}
$$

The half-line integral follows by setting $u=v_\phi^2/(2s)$ in the defining [Gamma function](../../../../../gamma-function.md) integral and requires $q>-1$. Matching its radial power and normalization to the [Mestel disk](../../../../../mestel-disk.md) yields the [rotating Mestel disk distribution function](../../../../../rotating-mestel-disk-distribution-function.md) parameters

$$
\boxed{q=\frac{v_0^2}{s}-1,\qquad F=A=\frac{\Sigma_0R_0^{-q}}{\sqrt\pi\,2^{q/2}s^{(q+2)/2}\Gamma((q+1)/2)}.}
$$

Since $v_0^2,s>0$, the required integrability condition is automatic. The amplitude uses the stated potential reference; changing the additive potential constant changes $A$ without changing the physical distribution.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 66](../../paper-66-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Use the usual minor and major symmetries of the [elastic stiffness tensor](../../../../../elastic-stiffness-tensor.md), positive density, and [strong ellipticity in elasticity](../../../../../strong-ellipticity-in-elasticity.md). For the plane [elastic wave](../../../../../elastic-wave.md) $u=a e^{ik(n\cdot x-vt)}$, substitution into momentum balance gives the [acoustic tensor](../../../../../acoustic-tensor.md) problem

$$
\Gamma_{ip}(n)a_p=\rho v^2a_i,\qquad
\Gamma_{ip}(n)=c_{ijpq}n_jn_q,\qquad
\boxed{\det(\Gamma(n)-\rho v^2I)=0.}
$$

The major symmetry makes $\Gamma$ a real [symmetric matrix](../../../../../symmetric-matrix.md). Moreover $a^{\mathsf T}\Gamma a=c_{ijpq}a_i n_j a_p n_q>0$ for nonzero $a$ under [strong ellipticity in elasticity](../../../../../strong-ellipticity-in-elasticity.md). Hence its three [eigenvalues](../../../../../eigenvalue.md) are positive and the three positive [wave speeds](../../../../../wave-speed.md) are real. Symmetry alone proves only reality of $v^2$: an unstable [isotropic](../../../../../isotropy.md) tensor with negative [shear modulus](../../../../../shear-modulus.md) has negative transverse $v^2$. The requested reality therefore uses stability as part of the physical elastic-solid assumption.

The [elastic slowness surface](../../../../../elastic-slowness-surface.md) consists of three sheets, with $s=n/v_\alpha(n)$, satisfying

$$
\det(c_{ijpq}s_js_q-\rho\delta_{ip})=0.
$$

It is centrosymmetric. Sheets can meet at degenerate polarizations; they need not be spherical or convex in an [anisotropic](../../../../../anisotropy.md) solid. The [group velocity](../../../../../group-velocity.md) is normal to the corresponding smooth sheet: for a sheet tangent $ds$, differentiation of $a^{\mathsf T}[c_{ijpq}s_js_q-\rho I]a=0$ gives $a_i c_{ijpq}a_p s_q\,ds_j=0$. The coefficient vector is proportional to the [group velocity](../../../../../group-velocity.md), so its scalar product with every tangent vanishes.

Fix horizontal [slowness](../../../../../slowness.md) $p=(n_1/c,n_2/c)$ and put $q=s_3$. Define

$$
T_{ip}=c_{i3p3},\qquad
R_{ip}=\sum_{\alpha=1}^2c_{i3p\alpha}p_\alpha,\qquad
Q_{ip}=\sum_{\alpha,\beta=1}^2c_{i\alpha p\beta}p_\alpha p_\beta.
$$

The symbol $p$ on a tensor index is an index, whereas $p_\alpha$ is a horizontal [slowness](../../../../../slowness.md) component. The vertical [slowness](../../../../../slowness.md) equation is the [vertical slowness sextic of an anisotropic solid](../../../../../vertical-slowness-sextic-of-an-anisotropic-solid.md)

$$
\boxed{\det\{Tq^2+(R+R^{\mathsf T})q+Q-\rho I\}=0.}
$$

The leading coefficient is $\det T>0$, so it is a degree-six polynomial with real coefficients. Nonreal roots occur in conjugate pairs, leaving between zero and six real roots counted with multiplicity. Generically the counts are $0,2,4,6$; a grazing repeated root can give an odd count of distinct real roots. Geometrically these are the intersections of a vertical line of fixed horizontal [slowness](../../../../../slowness.md) with the three sheets.

All four generic counts are actually possible in a stable material. For example, take $\rho=1$ and orthotropic Voigt stiffnesses

$$
C_{11}=25,\ C_{22}=16,\ C_{33}=9,\ C_{13}=-1,\ C_{12}=C_{23}=0,\quad
C_{44}=4,\ C_{55}=1,\ C_{66}=2.
$$

The stiffness matrix is positive definite. For horizontal [slowness](../../../../../slowness.md) $(p,0)$, the three diagonal acoustic equations are

$$
25p^2+q^2=1,\qquad 2p^2+4q^2=1,\qquad p^2+9q^2=1.
$$

The choices $p=0.1,0.3,0.8,1.2$ give respectively six, four, two and zero real vertical roots.

For the general depth-dependent amplitude, substitution of the horizontal harmonic factor yields

$$
T U''+i\omega(R+R^{\mathsf T})U'-\omega^2(Q-\rho I)U=0.
$$

For six simple roots $q_\ell$, choose nonzero null vectors $a_\ell$ of the corresponding matrix. The complete solution is

$$
\boxed{U(x_3)=\sum_{\ell=1}^6 A_\ell a_\ell e^{i\omega q_\ell x_3}.}
$$

Complex vertical roots give [evanescent waves](../../../../../evanescent-wave.md). At defective repeated roots the usual polynomial-in-depth factors multiplying exponentials must be included, or the solution can be defined by a limiting procedure.

To classify the modes, take $x_3$ positive downwards and $\omega>0$. The reduced [traction](../../../../../traction.md) for a mode is

$$
b_\ell=(Tq_\ell+R)a_\ell,\qquad \sigma_{i3}=i\omega b_{\ell,i}.
$$

Mechanical [energy](../../../../../energy.md) crosses a plane at rate $-\sigma_{i3}u_{i,t}$. Averaging the real harmonic fields uses $\langle\operatorname{Re}(f e^{-i\omega t})\operatorname{Re}(g e^{-i\omega t})\rangle=\operatorname{Re}(f g^*)/2$. With velocity amplitude $-i\omega a_\ell$ and [traction](../../../../../traction.md) amplitude $i\omega b_\ell$, the time-averaged vertical [acoustic energy flux](../../../../../acoustic-energy-flux.md) is

$$
J_{3,\ell}=\frac{\omega^2}{2}\operatorname{Re}(a_\ell^*b_\ell).
$$

For a real propagating mode, write its physical wavevector as $k=\omega(p_1,p_2,q)$. Differentiate $a^{\mathsf T}\Gamma(k)a=\rho\omega(k)^2a^{\mathsf T}a$ in $k_3$. The derivatives of $a$ cancel by the [eigenvalue](../../../../../eigenvalue.md) equation, while $a^{\mathsf T}(\partial_{k_3}\Gamma)a=2\omega a^{\mathsf T}(Tq+R)a$. Thus its vertical [group velocity](../../../../../group-velocity.md) and flux are

$$
g_{3,\ell}=\frac{a_\ell^{\mathsf T}(Tq_\ell+R)a_\ell}
{\rho\,a_\ell^{\mathsf T}a_\ell},\qquad
J_{3,\ell}=\frac12\rho\omega^2|a_\ell|^2g_{3,\ell}.
$$

Thus the [elastic mode classification by vertical energy flux](../../../../../elastic-mode-classification-by-vertical-energy-flux.md) is **upgoing if $J_3<0$, downgoing if $J_3>0$**. In [anisotropy](../../../../../anisotropy.md), the sign of vertical phase [slowness](../../../../../slowness.md) alone need not classify energy propagation. For evanescent modes, select $\operatorname{Im}q>0$ for decay into a downward half-space and $\operatorname{Im}q<0$ for decay into an upward half-space. Away from grazing and degeneracy, continuation from zero horizontal [slowness](../../../../../slowness.md), with a small radiation damping if needed, separates three outgoing modes on each side. Superpose only the appropriate three to construct the most general upgoing or downgoing field; limiting modes handle exceptional cases.

For a free surface at $x_3=0$ with solid occupying $x_3>0$, let $(q_0,a_0)$ be a unit-amplitude incident upgoing mode. The reflected field consists of the three downgoing propagating or depth-decaying modes:

$$
u=\left[a_0e^{i\omega q_0x_3}+
\sum_{r=1}^3 A_ra_re^{i\omega q_rx_3}\right]
e^{i\omega(p_1x_1+p_2x_2-t)}.
$$

Frequency and horizontal [slowness](../../../../../slowness.md) are common to all modes, by translation invariance of the surface. Zero surface [traction](../../../../../traction.md) imposes the three equations

$$
b_0+\sum_{r=1}^3A_rb_r=0,\qquad
B=(b_1,b_2,b_3).
$$

Hence the [free-surface anisotropic reflection amplitudes](../../../../../free-surface-anisotropic-reflection-amplitudes.md) are

$$
\boxed{(A_1,A_2,A_3)^{\mathsf T}=-B^{-1}b_0}
$$

whenever $B$ is invertible. This specifies mode conversion as well as reflection. If $B$ is singular, a nonzero outgoing homogeneous surface mode exists; these are surface-wave poles, including [Rayleigh waves](../../../../../rayleigh-wave.md) in the [isotropic](../../../../../isotropy.md) case. At such parameters one must use the appropriate limiting radiation solution and check solvability instead of assuming a unique finite inverse.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 47](../../paper-47-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

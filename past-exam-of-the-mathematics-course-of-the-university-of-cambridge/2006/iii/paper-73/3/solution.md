<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the stellar position second-moment tensor $I_{ij}=\int\rho x_ix_j\,d^3x$. This is the $I$ entering the [tensor virial theorem](../../../../../tensor-virial-theorem.md), rather than the engineering moment-of-inertia tensor $\operatorname{tr}(I)\mathbf1-I$. For a density pattern rotating steadily about its third principal axis, choose $t=0$ when its in-plane axes are principal axes. Then $I(0)=\operatorname{diag}(I_1,I_2,I_3)$ and

$$
I(t)=R(\Omega t)I(0)R(\Omega t)^T,\qquad R(\theta)=\begin{pmatrix}\cos\theta&-\sin\theta&0\\\sin\theta&\cos\theta&0\\0&0&1\end{pmatrix}.
$$

In particular, $I_{11}=I_1\cos^2\Omega t+I_2\sin^2\Omega t$, $I_{22}=I_1\sin^2\Omega t+I_2\cos^2\Omega t$, and $I_{12}=(I_1-I_2)\sin\Omega t\cos\Omega t$, while $I_{33}=I_3$ and $I_{13}=I_{23}=0$. Two differentiations at $t=0$ prove the [inertia-tensor acceleration of a steadily rotating stellar pattern](../../../../../inertia-tensor-acceleration-of-a-steadily-rotating-stellar-pattern.md):

$$
\boxed{\frac12\ddot I=\Omega^2\operatorname{diag}(I_{22}-I_{11},\ I_{11}-I_{22},\ 0).}
$$

Both the off-diagonal acceleration and the in-plane trace acceleration vanish at this instant.

Write $\mathbf u=\overline{\mathbf v}$ for the local mean streaming. The [stellar kinetic-energy tensor](../../../../../stellar-kinetic-energy-tensor.md), [stellar pressure-energy tensor](../../../../../stellar-pressure-energy-tensor.md), and [stellar potential-energy tensor](../../../../../stellar-potential-energy-tensor.md) have the conventions

$$
T_{ij}=\frac12\int\rho u_iu_j\,d^3x,\qquad \Pi_{ij}=\int\rho\overline{(v_i-u_i)(v_j-u_j)}\,d^3x,\qquad W_{ij}=-\int\rho x_i\partial_j\Phi\,d^3x.
$$

For an isolated self-gravitating system, $\tfrac12\ddot I_{ij}=2T_{ij}+\Pi_{ij}+W_{ij}$. Subtracting its second diagonal component from the first gives

$$
-2\Omega^2(I_{11}-I_{22})=(W_{11}-W_{22})+2(T_{11}-T_{22})+(\Pi_{11}-\Pi_{22}),
$$

so

$$
\boxed{\Omega^2=-\frac{(W_{11}-W_{22})+2(T_{11}-T_{22})+(\Pi_{11}-\Pi_{22})}{2(I_{11}-I_{22})}.}
$$

This quotient requires $I_{11}\ne I_{22}$. In an axisymmetric density distribution it becomes $0/0$: rotating the pattern about its symmetry axis does not change the density, and this equation cannot determine a pattern speed. Stellar streaming need not be rigid rotation with angular frequency $\Omega$.

Next add the first two diagonal virial equations and use the third. Their acceleration terms vanish, so

$$
W_{11}+W_{22}+2(T_{11}+T_{22})+\Pi_{11}+\Pi_{22}=0,\qquad W_{33}+2T_{33}+\Pi_{33}=0.
$$

For $T_{33}=0$, $\Pi_{33}=-W_{33}$. With the [planar virial trace](../../../../../planar-virial-trace.md) $\Pi_\perp=\Pi_{11}+\Pi_{22}$ and $W_\perp=W_{11}+W_{22}$, the prescribed mass-weighted quantities satisfy $\Pi_\perp=2M\sigma_0^2$, $2(T_{11}+T_{22})=MV_0^2$, and $1-\delta=2\Pi_{33}/\Pi_\perp$. Therefore $W_{33}=-(1-\delta)M\sigma_0^2$ and the planar equation becomes

$$
W_\perp+MV_0^2+2M\sigma_0^2=0.
$$

Eliminating $M\sigma_0^2$ gives

$$
\boxed{\frac{V_0^2}{\sigma_0^2}=(1-\delta)\frac{W_{11}+W_{22}}{W_{33}}-2.}
$$

The $\nu_0$ in the numerator of the PDF's displayed relation is a notation slip: the velocity subsequently defined is $V_0$. The relation follows from the traces, not from replacing a [galaxy](../../../../../galaxy-split.md) by a solid rotating body.

For the axisymmetric [oblate spheroid](../../../../../oblate-spheroid.md), rotational symmetry gives $\Pi_{11}=\Pi_{22}=M\sigma_0^2$, $\Pi_{33}=M\sigma_0^2(1-\delta)$ and zero integrated off-diagonal random stresses. A line-of-sight unit vector can be chosen as $\mathbf n=(\sin i,0,\cos i)$, with $i=0$ face-on. Contracting the random stress tensor with this vector gives the [inclination projection of an axisymmetric stellar velocity tensor](../../../../../inclination-projection-of-an-axisymmetric-stellar-velocity-tensor.md):

$$
\boxed{\sigma^2=\frac{n_i\Pi_{ij}n_j}{M}=\sigma_0^2\sin^2i+\sigma_0^2(1-\delta)\cos^2i=\sigma_0^2(1-\delta\cos^2i).}
$$

This is a mass-weighted random [velocity dispersion](../../../../../velocity-dispersion.md) after subtracting streaming, with consistent aperture weights. Along the projected major axis, azimuthal streaming lies along the direction whose line-of-sight projection is $\sin i$; a rotation amplitude $V_0$ consequently projects as

$$
\boxed{V_r=V_0\sin i.}
$$

There is a necessary observational convention here. The globally defined $V_0^2=2(T_{11}+T_{22})/M$ is a streaming mean square. The displayed amplitude relation holds if the [rotation curve](../../../../../galaxy-rotation-curve.md) is constant, or if the measured rotation-amplitude statistic is weighted consistently to represent this intrinsic quantity. Axisymmetry alone does not equate an arbitrary observed peak rotation to the global $V_0$. If $V_r$ instead means the full-aperture line-of-sight streaming root-mean-square, azimuthal averaging yields

$$
\langle u_{\rm los}^2\rangle=\sin^2i\,\frac{2T_{11}}M=\frac12V_0^2\sin^2i,
$$

and the corresponding root-mean-square is $V_0\sin i/\sqrt2$. Keeping amplitude and root-mean-square distinct prevents a spurious factor of two in the [kinetic energy](../../../../../kinetic-energy.md).

Finally, let the intrinsic equatorial and polar semiaxes be $a$ and $c$, and put $q_t=c/a=1-\epsilon_t$. An intrinsic boundary has $(x^2+y^2)/a^2+z^2/c^2=1$. Its sky minor-axis coordinate is $Y=y\cos i-z\sin i$. Eliminating the line-of-sight coordinate, or maximizing $Y$ on this ellipse, gives the projected minor semiaxis $\sqrt{a^2\cos^2i+c^2\sin^2i}$; the major semiaxis remains $a$. Thus the [projected axis ratio of an oblate spheroid](../../../../../projected-axis-ratio-of-an-oblate-spheroid.md) is

$$
q_a^2=\cos^2i+q_t^2\sin^2i,\qquad q_a=1-\epsilon_a.
$$

Subtracting from unity proves

$$
\boxed{\epsilon_a(2-\epsilon_a)=\epsilon_t(2-\epsilon_t)\sin^2i.}
$$

The face-on limit is round with zero projected rotation amplitude; the edge-on limit reveals the intrinsic flattening and in-plane random [velocity dispersion](../../../../../velocity-dispersion.md). These limits check both the geometry and the convention for inclination.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 73](../../paper-73-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

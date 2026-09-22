<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [linearized coordinate gauge transformation](../../../../../linearized-coordinate-gauge-transformation.md) changes the identification of points of the perturbed [spacetime](../../../../../spacetime.md) with its [Minkowski spacetime](../../../../../minkowski-spacetime.md) background. With $x'^i=x^i+\epsilon\xi^i$, the same physical metric has perturbation

$$
h'_{ij}=h_{ij}-\partial_i\xi_j-\partial_j\xi_i.
$$

These changes are coordinate freedom, not extra physical [gravitational wave polarizations](../../../../../gravitational-wave-polarization.md). Raising indices with $\eta$, define $h=\eta^{ij}h_{ij}$ and the [trace-reversed metric perturbation](../../../../../trace-reversed-metric-perturbation.md) $\bar h_{ij}=h_{ij}-\eta_{ij}h/2$. Then

$$
\bar h'_{ij}=\bar h_{ij}-\partial_i\xi_j-\partial_j\xi_i+\eta_{ij}\partial_k\xi^k.
$$

The first-order [Levi-Civita connection](../../../../../levi-civita-connection.md) is $\Gamma^{(1)k}{}_{ij}=\tfrac12\eta^{k\ell}(\partial_ih_{j\ell}+\partial_jh_{i\ell}-\partial_\ell h_{ij})$. Contracting the [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) in the stated convention gives

$$
R^{(1)}_{ij}=\tfrac12\left(\partial_i\partial_kh^k{}_j+\partial_j\partial_kh^k{}_i-\Box h_{ij}-\partial_i\partial_jh\right),
\qquad R^{(1)}=\partial_i\partial_jh^{ij}-\Box h.
$$

Put $A_j=\partial^i\bar h_{ij}$. The corresponding [Einstein tensor](../../../../../einstein-tensor.md) is

$$
G^{(1)}_{ij}=-\tfrac12\Box\bar h_{ij}
+\tfrac12\left(\partial_iA_j+\partial_jA_i-\eta_{ij}\partial^kA_k\right).
$$

Under the [linearized coordinate gauge transformation](../../../../../linearized-coordinate-gauge-transformation.md), $A'_j=A_j-\Box\xi_j$. Choosing a solution of $\Box\xi_j=A_j$ imposes [Lorenz gauge in linearized gravity](../../../../../lorenz-gauge-in-linearized-gravity.md), $A'_j=0$. Thus the vacuum [Einstein field equations](../../../../../einstein-field-equations.md) reduce to

$$
\boxed{\partial^i\bar h_{ij}=0,\qquad\Box\bar h_{ij}=0.}
$$

There remains [residual gauge symmetry of linearized gravity](../../../../../residual-gauge-symmetry-of-linearized-gravity.md) with $\Box\xi_j=0$.

For the transverse profiles, write both symmetric off-diagonal entries as $h_{xy}=h_{yx}=h_\times(t-z)$ and the diagonal entries as $h_{xx}=-h_{yy}=h_+(t-z)$. The [trace-reversed metric perturbation](../../../../../trace-reversed-metric-perturbation.md) has zero trace and therefore equals $h$. Its divergence vanishes: its only nonzero index directions are $x,y$, while its coefficients depend only on $t-z$. Also $(-\partial_t^2+\partial_z^2)F(t-z)=0$ for every twice differentiable profile $F$. These are consequently [plane gravitational waves in linearized gravity](../../../../../plane-gravitational-wave-in-linearized-gravity.md) in [transverse-traceless gauge](../../../../../transverse-traceless-gauge.md), with the two independent [gravitational wave polarizations](../../../../../gravitational-wave-polarization.md) $h_+$ and $h_\times$.

To calculate the detector response, use a [parallel-propagated orthonormal frame](../../../../../parallel-propagated-orthonormal-frame.md) along the centre of a short nonrotating stick. To first order its clock reads $t$, and the tidal curvature is

$$
R_{A0B0}=-\frac\epsilon2\ddot h_{AB}+O(\epsilon^2),\qquad A,B\in\{x,y\}.
$$

For a [sliding-bead gravitational wave detector](../../../../../sliding-bead-gravitational-wave-detector.md), the stick constrains transverse motion but supplies no axial restoring force. Projecting [geodesic deviation](../../../../../geodesic-deviation.md) along an $x$-directed stick gives

$$
\ddot L=\frac\epsilon2\ddot h_+(t-z_0)L_0+O(\epsilon^2).
$$

Here $L$ is the proper separation and $L_0=L(t_0)$, with $\dot L(t_0)=0$. Integrating with those actual initial conditions yields

$$
\boxed{L(t)=L_0\left[1+\frac\epsilon2\left(h_+(t-z_0)-h_+(t_0-z_0)
-(t-t_0)\dot h_+(t_0-z_0)\right)\right]+O(\epsilon^2).}
$$

For beads at rest before an incident wave, both initial profile terms vanish and the familiar result is $\boxed{L(t)=L_0[1+\epsilon h_+(t-z_0)/2]+O(\epsilon^2)}$. The cross polarization produces a transverse tidal force, balanced by the guide, and no axial first-order displacement in this orientation. In [transverse-traceless gauge](../../../../../transverse-traceless-gauge.md) the same plus response can be read from the proper line element, $d\ell=\sqrt{1+\epsilon h_+}\,dx$; coordinate distances alone are not measured distances. When a cross polarization is present, keeping the guide physically nonrotating may require transverse coordinate adjustments, which do not change the axial answer at this order.

For a $z$-directed stick, $R_{z0z0}=0$ and the wave is transverse. Therefore **beads initially at rest retain their proper separation to first order**: $L(t)=L_0+O(\epsilon^2)$. The tidal calculation is the usual linear detector limit, with bead spacing small compared with the wavelength; it does not treat a macroscopic rigid body as exactly rigid over arbitrary relativistic distances.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 52](../../paper-52-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

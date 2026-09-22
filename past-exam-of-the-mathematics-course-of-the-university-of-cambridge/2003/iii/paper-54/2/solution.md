<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Work to first order in a [metric perturbation](../../../../../linearized-gravity.md) $g_{ab}=\eta_{ab}+h_{ab}$, with $\eta=\operatorname{diag}(1,-1,-1,-1)$, raising perturbation indices with $\eta$ and discarding quadratic terms. The [Christoffel symbols](../../../../../christoffel-symbol.md) are

$$
\Gamma^{a(1)}{}_{bc}=\frac12\eta^{ad}(\partial_bh_{dc}+\partial_ch_{db}-\partial_dh_{bc}).
$$

Using the printed curvature convention gives the [linearized Riemann curvature operator](../../../../../linearized-riemann-curvature-operator.md)

$$
R^{(1)}_{abcd}=\frac12(\partial_b\partial_dh_{ac}+\partial_a\partial_ch_{bd}-\partial_a\partial_dh_{bc}-\partial_b\partial_ch_{ad}).
$$

For definiteness contract $R_{bd}=R^a{}_{bad}$. The corresponding first-order [Ricci tensor](../../../../../ricci-tensor.md) is

$$
R^{(1)}_{ab}=\frac12(\partial_a\partial_bh+\Box h_{ab}-\partial_a\partial^ch_{cb}-\partial_b\partial^ch_{ca}),\qquad\Box=\partial_t^2-\Delta.
$$

This is the reversed sign convention specified in [curvature-sign convention in Killing derivative identities](../../../../../curvature-sign-convention-in-killing-derivative-identities.md); the vacuum equation is unaffected by an overall curvature sign.

An infinitesimal passive coordinate change $x'^a=x^a+\xi^a$ changes the perturbation by $\delta h_{ab}=-\partial_a\xi_b-\partial_b\xi_a$. Substitution into $R^{(1)}$ gives zero change, since partial derivatives commute. Equivalently the change in curvature is the Lie derivative of the background curvature, which vanishes in [Minkowski spacetime](../../../../../minkowski-spacetime.md). Thus linearized curvature, and the linearized [Weyl tensor](../../../../../weyl-tensor.md) in vacuum, are gauge-invariant tidal observables, whereas individual components of $h$ are generally gauge dependent.

The [trace-reversed metric perturbation](../../../../../trace-reversed-metric-perturbation.md) $\bar h_{ab}=h_{ab}-\eta_{ab}h/2$ transforms by $\delta\bar h_{ab}=-\partial_a\xi_b-\partial_b\xi_a+\eta_{ab}\partial_c\xi^c$. Its divergence changes by $-\Box\xi_b$. Solving $\Box\xi_b=\partial^a\bar h_{ab}$ therefore imposes [Lorenz gauge in linearized gravity](../../../../../lorenz-gauge-in-linearized-gravity.md), $\partial^a\bar h_{ab}=0$. With the stated sign convention the [Einstein tensor](../../../../../einstein-tensor.md) is

$$
G^{(1)}_{ab}=\frac12[\Box\bar h_{ab}-\partial_a\partial^c\bar h_{cb}-\partial_b\partial^c\bar h_{ca}+\eta_{ab}\partial^c\partial^d\bar h_{cd}],
$$

so the linearized vacuum field equation becomes $\boxed{\Box\bar h_{ab}=0}$. The [residual gauge symmetry of linearized gravity](../../../../../residual-gauge-symmetry-of-linearized-gravity.md) has $\Box\xi_a=0$. This makes a hyperbolic evolution problem after the gauge condition and its initial consistency constraints have been imposed.

To separate actual gauge invariants from a gauge choice, use [gauge-invariant Minkowski perturbations](../../../../../gauge-invariant-scalar-vector-tensor-perturbations-of-minkowski-spacetime.md). For spatial indices contracted with $\delta_{ij}$, decompose

$$
h_{00}=2A,\quad h_{0i}=\partial_iB+B_i,\quad h_{ij}=2C\delta_{ij}+2(\partial_i\partial_j-\delta_{ij}\Delta/3)E+\partial_iE_j+\partial_jE_i+h_{ij}^{\rm TT},
$$

where $\partial_iB_i=\partial_iE_i=0$, $\partial_ih_{ij}^{\rm TT}=0$ and $h_{ii}^{\rm TT}=0$. Spatial falloff or Fourier-mode conventions fix the decomposition. Write $\xi^0=\tau$ and $\xi^i=\partial_iL+L_i$ with $\partial_iL_i=0$. Direct substitution in the gauge change gives

$$
\delta A=-\dot\tau,\quad\delta B=\dot L-\tau,\quad\delta C=\Delta L/3,\quad\delta E=L,\quad\delta B_i=\dot L_i,\quad\delta E_i=L_i,\quad\delta h_{ij}^{\rm TT}=0.
$$

Hence the invariant combinations are

$$
\boxed{\Phi=A-\dot B+\ddot E,\qquad\Psi=C-\Delta E/3,\qquad V_i=B_i-\dot E_i,\qquad h_{ij}^{\rm TT}.}
$$

A representative with $E=E_i=B=0$ has $h_{00}=2\Phi$, $h_{0i}=V_i$ and $h_{ij}=2\Psi\delta_{ij}+h_{ij}^{\rm TT}$. The explicit [vacuum constraints for gauge-invariant Minkowski perturbations](../../../../../vacuum-constraints-for-gauge-invariant-minkowski-perturbations.md) follow from

$$
G^{(1)}_{00}=-2\Delta\Psi,\qquad G^{(1)}_{0i}=-2\partial_i\dot\Psi-\tfrac12\Delta V_i,
$$



$$
G^{(1)}_{ij}=(\partial_i\partial_j-\delta_{ij}\Delta)(\Phi-\Psi)-2\delta_{ij}\ddot\Psi-\tfrac12(\partial_i\dot V_j+\partial_j\dot V_i)+\tfrac12\Box h_{ij}^{\rm TT}.
$$

For a nonzero spatial Fourier mode, or regular decaying fields on all space, $G_{00}=0$ forces $\Psi=0$, then $G_{0i}=0$ forces $V_i=0$, and the spatial trace gives $\Delta\Phi=0$, hence $\Phi=0$. Only $\Box h_{ij}^{\rm TT}=0$ remains. This removal of the scalar and vector sectors does not exclude singular Coulomb perturbations outside a source, boundary-driven harmonic potentials or spatially homogeneous modes; those require separate boundary and gauge conventions.

For a propagating plane mode $h\propto e^{ik_ax^a}$, the wave equation gives $k^ak_a=0$. A transverse-traceless spatial tensor perpendicular to a fixed propagation direction has two independent components. For propagation along $z$, define the physical strain $H_{ij}=-h_{ij}^{\rm TT}$ in this mostly-minus convention, so the spatial line element is $(\delta_{ij}+H_{ij})dx^idx^j$. It has the form

$$
H_{ij}(t,z)=\begin{pmatrix}H_+(t-z)&H_\times(t-z)&0\\H_\times(t-z)&-H_+(t-z)&0\\0&0&0\end{pmatrix}.
$$

These are the two [gravitational wave polarizations](../../../../../gravitational-wave-polarization.md), [plus polarization](../../../../../plus-polarization.md) and [cross polarization](../../../../../cross-polarization.md). A rotation in the transverse plane rotates the polarization pair through twice the angle; cross is plus rotated through $45$ degrees. Lorenz constraints and residual gauge freedom give the same count: ten symmetric metric components minus four constraints and four gauge freedoms leave two radiative degrees of freedom.

In [transverse-traceless gauge](../../../../../transverse-traceless-gauge.md), particles initially at rest keep fixed spatial coordinates since $\Gamma^a{}_{00}=0$, but their measured separation changes. For a short separation of length $L$ in unit direction $n$, $\delta L/L=H_{ij}n^in^j/2$. The gauge-invariant curvature gives the corresponding [geodesic deviation](../../../../../geodesic-deviation.md):

$$
R^{i(1)}{}_{00j}=\tfrac12\ddot h_{ij}^{\rm TT}=-\tfrac12\ddot H_{ij},\qquad\ddot\xi^i=-R^{i(1)}{}_{00j}\xi^j=\tfrac12\ddot H_{ij}\xi^j.
$$

Here the last equation is in a freely falling orthonormal frame, with the printed reversed curvature convention. Coordinate separation and physical separation must not be confused. The linearized vacuum equations describe propagation and tidal measurements; wave energy transfer and an effective wave [stress-energy tensor](../../../../../stress-energy-tensor.md) arise at quadratic order, beyond the linear approximation.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 54](../../paper-54-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

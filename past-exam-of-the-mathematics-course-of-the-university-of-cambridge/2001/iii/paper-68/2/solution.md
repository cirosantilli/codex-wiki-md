<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use $c=1$, background [Minkowski spacetime](../../../../../minkowski-spacetime.md) [metric tensor](../../../../../metric-tensor.md) $\eta_{ab}=\operatorname{diag}(1,-1,-1,-1)$, and $g_{ab}=\eta_{ab}+h_{ab}$ with small [metric perturbation](../../../../../linearized-gravity.md). All indices and [derivatives](../../../../../derivative.md) in this [linear](../../../../../linearity.md) approximation use $\eta$. The [linearized inverse metric](../../../../../linearized-inverse-metric.md) is $\eta^{ab}-h^{ab}$, and the [linearized Levi-Civita connection](../../../../../linearized-levi-civita-connection.md) is

$$
\Gamma^a{}_{bc}=\frac12\eta^{ad}
(\partial_bh_{cd}+\partial_ch_{bd}-\partial_dh_{bc}).
$$

Define the [trace-reversed metric perturbation](../../../../../trace-reversed-metric-perturbation.md) $\bar h_{ab}=h_{ab}-\eta_{ab}h/2$, with $h=\eta^{ab}h_{ab}$.

An infinitesimal coordinate change $x'^a=x^a+\xi^a$ gives the [linearized coordinate gauge transformation](../../../../../linearized-coordinate-gauge-transformation.md)

$$
h'_{ab}=h_{ab}-\partial_a\xi_b-\partial_b\xi_a,\qquad
\bar h'_{ab}=\bar h_{ab}-\partial_a\xi_b-\partial_b\xi_a
+\eta_{ab}\partial_c\xi^c.
$$

The [metric perturbation](../../../../../linearized-gravity.md) therefore has redundant components. The [gauge invariance of the linearized Riemann tensor](../../../../../gauge-invariance-of-the-linearized-riemann-tensor.md) follows because its change contains third [derivatives](../../../../../derivative.md) of $\xi$ cancelling by commutation of [partial derivatives](../../../../../partial-derivative.md). Conversely, [flat linearized metric perturbations are locally pure gauge](../../../../../flat-linearized-metric-perturbations-are-locally-pure-gauge.md) on a [contractible](../../../../../contractible-space.md) patch. Thus linearized [curvature](../../../../../curvature.md), rather than a particular coordinate value of $h$, detects the physical disturbance. Gauge freedom can also be restricted by global [topology](../../../../../topology-split.md) or [boundary conditions](../../../../../boundary-condition.md).

Keeping the paper's [curvature sign convention](../../../../../curvature-sign-convention.md), its [linearized Ricci tensor and scalar](../../../../../linearized-ricci-tensor-and-scalar.md) are

$$
R^{(1)}_{ab}=\frac12\left[
\Box h_{ab}+\partial_a\partial_bh
-\partial_a\partial^ch_{bc}-\partial_b\partial^ch_{ac}\right],
\qquad R^{(1)}=\Box h-\partial_a\partial_bh^{ab}.
$$

These are the negatives of the alternative frequently used [curvature](../../../../../curvature.md) convention. Put $v_b=\partial^a\bar h_{ab}$. The [Linearized Einstein equations](../../../../../linearized-einstein-equations.md) in vacuum are

$$
G^{(1)}_{ab}=\frac12\left[
\Box\bar h_{ab}-\partial_av_b-\partial_bv_a
+\eta_{ab}\partial^cv_c\right]=0,\qquad
\Box=\partial_t^2-\nabla^2.
$$

Under a gauge change $v_b\mapsto v_b-\Box\xi_b$, so solving $\Box\xi_b=v_b$ imposes the [Lorenz gauge in linearized gravity](../../../../../lorenz-gauge-in-linearized-gravity.md). The field equations then become $\Box\bar h_{ab}=0$. The remaining [residual gauge symmetry of linearized gravity](../../../../../residual-gauge-symmetry-of-linearized-gravity.md) has $\Box\xi_b=0$; Lorenz gauge does not exhaust the coordinate freedom.

A [Fourier mode](../../../../../fourier-mode.md) $\bar h_{ab}=A_{ab}e^{ik_cx^c}$ obeys $k^ak_a=0$ and $k^aA_{ab}=0$. Hence the [plane gravitational waves in linearized gravity](../../../../../plane-gravitational-wave-in-linearized-gravity.md) propagate on the background [light cones](../../../../../light-cone.md). Four transversality conditions and four residual gauge amplitudes leave $10-4-4=2$ physical degrees of freedom. The [explicit plane-wave reduction to transverse-traceless gauge](../../../../../explicit-plane-wave-reduction-to-transverse-traceless-gauge.md) can set $h_{0a}=0$, spatial [trace](../../../../../matrix-trace.md) zero and $k^ih_{ij}=0$. For a wave in the $z$ direction, write its physical spatial strain as $H_{ij}=-h_{ij}$, so the spatial [metric tensor](../../../../../metric-tensor.md) is $-(\delta_{ij}+H_{ij})$:

$$
H_{ij}(t-z)=
\begin{pmatrix}
H_+&H_\times&0\\
H_\times&-H_+&0\\
0&0&0
\end{pmatrix}.
$$

There are **two [gravitational wave polarizations](../../../../../gravitational-wave-polarization.md)**, [plus polarization](../../../../../plus-polarization.md) and [cross polarization](../../../../../cross-polarization.md). Rotating transverse axes through $\theta$ rotates their amplitude pair through $2\theta$. Nonconstant profiles with nonzero second [derivative](../../../../../derivative.md) have nonzero linearized [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md) and cannot be removed as pure gauge.

The [TT coordinate separation and measured separation](../../../../../tt-coordinate-separation-and-measured-separation.md) distinction explains a detector's response. Freely falling particles initially at rest can keep fixed TT coordinates, since $\Gamma^a{}_{00}=0$, while their proper separation changes. For a short arm along a unit vector $n$,

$$
\frac{\delta L}{L}=\frac12H_{ij}n^in^j,\qquad
\frac{d^2\delta L}{dt^2}=\frac12\ddot H_{ij}n^in^jL.
$$

This is the tidal response described by [geodesic deviation](../../../../../geodesic-deviation.md); coordinate motion by itself is not the measured signal.

Finally, gravitational-wave energy is second order in the perturbation, so it is absent from a first-order vacuum equation. In a short-wavelength averaging regime the [averaged stress-energy of transverse gravitational waves](../../../../../averaged-stress-energy-of-transverse-gravitational-waves.md) is

$$
t^{\rm GW}_{ab}=\frac{1}{32\pi G}
\left\langle\partial_aH_{ij}\partial_bH_{ij}\right\rangle.
$$

For a plane wave its [energy flux](../../../../../energy-flux.md) is $(16\pi G)^{-1}\langle\dot H_+^2+\dot H_\times^2\rangle$. The averaging scale and weak-field assumptions matter: this does not assign a coordinate-independent local gravitational [energy density](../../../../../energy-density.md) to an arbitrary first-order perturbation.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 68](../../paper-68-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

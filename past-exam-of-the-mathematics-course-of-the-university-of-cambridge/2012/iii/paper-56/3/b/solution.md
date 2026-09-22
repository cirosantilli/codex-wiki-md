<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a nonzero, nonconstant vacuum [plane gravitational wave in linearized gravity](../../../../../../plane-gravitational-wave-in-linearized-gravity.md) with real wave covector $k$, the [Linearized Einstein equations](../../../../../../linearized-einstein-equations.md) and [Lorenz gauge in linearized gravity](../../../../../../lorenz-gauge-in-linearized-gravity.md) require

$$
\boxed{H_{\mu\nu}=H_{\nu\mu},\qquad k^\mu H_{\mu\nu}=0,\qquad k^\mu k_\mu=0.}
$$

The zero-amplitude solution places no restriction on $k$; a constant mode $k=0$ is not a propagating wave. Under the sign convention for the infinitesimal change specified here, the [trace-reversed metric perturbation](../../../../../../trace-reversed-metric-perturbation.md) changes by

$$
\delta\bar h_{\mu\nu}=\partial_\mu\xi_\nu+\partial_\nu\xi_\mu-\eta_{\mu\nu}\partial_\rho\xi^\rho,\qquad \partial^\mu\delta\bar h_{\mu\nu}=\Box\xi_\nu.
$$

Thus the [residual gauge symmetry of linearized gravity](../../../../../../residual-gauge-symmetry-of-linearized-gravity.md) is characterized by **$\Box\xi_\nu=0$**. The proposed plane-wave form obeys this for every constant complex $X_\nu$, because $k$ is null. Changing the sign used to name $\xi$ would reverse both gauge formulas, with no physical consequence.

Rotate the spatial axes so the wave propagates along $+z$, choosing $k_\mu=(-\omega,0,0,\omega)$ with $\omega>0$. The [Lorenz gauge in linearized gravity](../../../../../../lorenz-gauge-in-linearized-gravity.md) says $H_{3\nu}=-H_{0\nu}$; in particular $H_{03}=-H_{00}$, $H_{33}=H_{00}$ and $H_{3i}=-H_{0i}$ for $i=1,2$. The amplitude change is

$$
\delta H_{\mu\nu}=i\bigl(k_\mu X_\nu+k_\nu X_\mu-\eta_{\mu\nu}k^\rho X_\rho\bigr).
$$

Choose

$$
X_1=\frac{H_{01}}{i\omega},\qquad X_2=\frac{H_{02}}{i\omega},\qquad X_3-X_0=\frac{iH_{00}}{\omega},\qquad X_0+X_3=\frac{H_{11}+H_{22}}{2i\omega}.
$$

Indeed, $\delta H_{00}=i\omega(X_3-X_0)$ and $\delta H_{0i}=-i\omega X_i$ cancel the time components, while $\delta H_{11}=\delta H_{22}=-i\omega(X_0+X_3)$ cancels the transverse trace. The preserved [Lorenz gauge in linearized gravity](../../../../../../lorenz-gauge-in-linearized-gravity.md) then cancels all longitudinal components. This is an [explicit plane-wave reduction to transverse-traceless gauge](../../../../../../explicit-plane-wave-reduction-to-transverse-traceless-gauge.md), yielding

$$
\boxed{H'_{\mu\nu}=\begin{pmatrix}0&0&0&0\\0&H_+&H_\times&0\\0&H_\times&-H_+&0\\0&0&0&0\end{pmatrix},\qquad H_+=\frac{H_{11}-H_{22}}2,\quad H_\times=H_{12}.}
$$

The [trace-reversed metric perturbation](../../../../../../trace-reversed-metric-perturbation.md) has zero trace in this [transverse-traceless gauge](../../../../../../transverse-traceless-gauge.md), so $h'=\bar h'$. The null dispersion relation is $\omega^2=|\mathbf k|^2$, giving the speed of light. Only components perpendicular to the direction of propagation remain, and the two independent amplitudes give the plus and cross [gravitational wave polarizations](../../../../../../gravitational-wave-polarization.md).

These are physical transverse tidal distortions, rather than just a convenient display of the [metric perturbation](../../../../../../linearized-gravity.md): in [transverse-traceless gauge](../../../../../../transverse-traceless-gauge.md), $R^{(1)}_{0i0j}=-\tfrac12\partial_t^2h'_{ij}$, so a freely falling detector has $\ddot S^i=\tfrac12\ddot h'_{ij}S^j$ at first order. There is no longitudinal tidal acceleration. The plus polarization stretches one transverse axis while compressing the other; the cross polarization does the same along axes rotated by $\pi/4$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 56](../../../paper-56-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

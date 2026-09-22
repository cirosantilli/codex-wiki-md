<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $A,B\in\{1,2\}$ and write $h_{AB}=H_{AB}e^{ik\cdot x}$, where $H_{11}=H_+$, $H_{22}=-H_+$ and $H_{12}=H_{21}=H_\times$. Physical fields are the real parts. Use $c=1$ here, and take the initial separation at equal time, so $L^0=0$. For propagation in the positive $x^3$ direction one may set $k_\mu=(-\omega,0,0,\omega)$; only $k_0^2=\omega^2$ enters the answer.

The [linearized Levi-Civita connection](../../../../../../linearized-levi-civita-connection.md) in this [transverse-traceless gauge](../../../../../../transverse-traceless-gauge.md) has the potentially nonzero components

$$
\Gamma^0{}_{AB}=\frac12\partial_0h_{AB},\qquad
\Gamma^3{}_{AB}=-\frac12\partial_3h_{AB},\qquad
\Gamma^A{}_{0B}=\Gamma^A{}_{B0}=\frac12\partial_0h_{AB},\qquad
\Gamma^A{}_{3B}=\Gamma^A{}_{B3}=\frac12\partial_3h_{AB},
$$

with all others zero to this order. In particular $\Gamma^\mu{}_{00}=0$, so a particle initially at rest has fixed spatial coordinates in [transverse-traceless gauge](../../../../../../transverse-traceless-gauge.md), and $t$ equals its [proper time](../../../../../../proper-time.md). Expanding the [Riemann curvature tensor](../../../../../../riemann-curvature-tensor.md) gives

$$
R^{(1)}_{\mu\nu\rho\sigma}=\frac12\bigl(\partial_\rho\partial_\nu h_{\mu\sigma}+\partial_\sigma\partial_\mu h_{\nu\rho}-\partial_\rho\partial_\mu h_{\nu\sigma}-\partial_\sigma\partial_\nu h_{\mu\rho}\bigr),
\qquad R_{0A0B}^{(1)}=-\frac12\ddot h_{AB},
\qquad R^A{}_{00B}^{(1)}=\frac12\ddot h_{AB}.
$$

The plus sign in the last expression agrees with $R(T,S)T$ in the [geodesic deviation](../../../../../../geodesic-deviation.md) convention above.

For the separation measured in a [parallel-propagated orthonormal frame](../../../../../../parallel-propagated-orthonormal-frame.md), write $S^{\hat\mu}=L^{\hat\mu}+\xi^{\hat\mu}$. The frame removes the connection terms from the time derivative, so the [geodesic deviation](../../../../../../geodesic-deviation.md) equation reduces to $\ddot\xi^{\hat A}=R^{\hat A}{}_{\hat0\hat0\hat B}L^{\hat B}=\ddot h_{AB}L^{\hat B}/2$ at first order. **The observable transverse relative acceleration is**

$$
\boxed{\begin{aligned}
\ddot\xi^{\hat0}&=0,\qquad \ddot\xi^{\hat3}=0,\\
\ddot\xi^{\hat1}&=-\frac{k_0^2}{2}(H_+L^{\hat1}+H_\times L^{\hat2})e^{ik\cdot x},\\
\ddot\xi^{\hat2}&=-\frac{k_0^2}{2}(H_\times L^{\hat1}-H_+L^{\hat2})e^{ik\cdot x}.
\end{aligned}}
$$

These are the [plus polarization](../../../../../../plus-polarization.md) and [cross polarization](../../../../../../cross-polarization.md) tidal patterns; there is no longitudinal acceleration. The curvature is evaluated along the reference worldline, and replacing $S$ by $L$ on the right changes only second-order terms. This is the infinitesimal-separation approximation intrinsic to [geodesic deviation](../../../../../../geodesic-deviation.md).

There is an important component distinction if the symbols $L^\mu+\xi^\mu$ are instead interpreted literally in the [transverse-traceless gauge](../../../../../../transverse-traceless-gauge.md) coordinate basis. Expanding the left side, rather than replacing a [covariant derivative](../../../../../../covariant-derivative.md) by an ordinary derivative, gives

$$
(\nabla_T\nabla_TS)^\mu=\ddot\xi_{\rm coord}^{\mu}+\partial_0\Gamma^\mu{}_{0j}L^j+O(\epsilon^2),
\qquad
R^\mu{}_{00j}L^j=\partial_0\Gamma^\mu{}_{0j}L^j+O(\epsilon^2).
$$

Thus **in TT coordinates**

$$
\boxed{\ddot\xi_{\rm coord}^{\mu}=0.}
$$

With zero initial coordinate displacement and velocity, $\xi_{\rm coord}=0$ throughout. This does not remove the physical [gravitational wave](../../../../../../gravitational-wave.md) strain. To first order an [orthonormal coframe in spacetime](../../../../../../orthonormal-coframe-in-spacetime.md) along the reference worldline is $\vartheta^{\hat A}=(\delta^A{}_B+h_{AB}/2)dx^B$; its dual frame is parallel propagated because $\partial_0(\delta^A{}_B-h_{AB}/2)+\Gamma^A{}_{0B}=0$. Hence

$$
S^{\hat A}=S^A+\frac12h_{AB}L^B,
\qquad \xi^{\hat A}=\xi_{\rm coord}^A+\frac12h_{AB}L^B,
$$

after choosing the initial flat-frame reference. The [TT coordinate separation and measured separation](../../../../../../tt-coordinate-separation-and-measured-separation.md) distinction accounts exactly for the apparently different accelerations. In a region initially free of the wave, the measured displacement is $\xi^{\hat A}=h_{AB}L^{\hat B}/2$ with the corresponding initial conditions.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 309](../../../paper-309-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

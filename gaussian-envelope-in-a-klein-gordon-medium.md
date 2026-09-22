# Gaussian envelope in a Klein-Gordon medium

↑ **Parent:** [Wave packet](wave-packet.md)

For the stipulated [Klein-Gordon packet velocities](klein-gordon-packet-velocities.md), take the original normalized spectral amplitude

$$
a(k)=\frac{1}{\sqrt{2\pi}\sigma}\exp\!\left[-\frac{(k-k_0)^2}{2\sigma^2}\right],\qquad
\psi(x,t)=\int_{\mathbb R}a(k)e^{i[kx-\omega(k)t]}\,dk,
$$

with $k_0>0$ and $0<\sigma\ll k_0$. Here $\sigma$ is the width of the spectral amplitude, not the [standard deviation](standard-deviation.md) of its squared magnitude. Initially $\psi(x,0)=e^{-\sigma^2x^2/2}e^{ik_0x}$, a [Gaussian function](gaussian-function.md) multiplying a [carrier wave](carrier-wave.md). Taking $u=\operatorname{Re}\psi$ gives a real solution of the [Klein-Gordon equation](klein-gordon-equation.md) with the corresponding initial [velocity](velocity.md). The tiny negative-$k$ tail is retained in this exact integral; the statement that it is mainly right-going is a narrow-spectrum approximation, not a claim of strictly positive [wavenumbers](wavenumber.md).

<a id="image-original-klein-gordon-packet-evolution-exact-spectral-integral-slower-envelope-and-carrier-phase-reference"></a>
![](klein-gordon-gaussian-carrier-envelope-evolution.png)

**[Figure 14](#image-original-klein-gordon-packet-evolution-exact-spectral-integral-slower-envelope-and-carrier-phase-reference). Original Klein-Gordon packet evolution: exact spectral integral, slower envelope and carrier phase reference**.

The dimensionless figure uses $c=\omega_0=k_0=1$ and $\sigma=0.18$ at $t=0,4,8$. Blue curves are $\operatorname{Re}\psi$, orange bounds are $\pm|\psi|$, and the marked [carrier wave](carrier-wave.md) reference is $x=v_pt$; it need not be a crest of the full wavefield. The dashed envelope-centre reference $x=v_gt$ is a leading approximation. These are calculated curves, not experimental records. The exact [dispersion relation](dispersion-relation.md) makes the packet slightly asymmetric; a quadratic approximation predicts symmetric broadening about $v_gt$.

The first-order [Taylor expansion](taylor-expansion.md) translates the initial [wave envelope](envelope-waves.md) without changing its shape. Retaining curvature instead gives

$$
\omega(k)\simeq\omega_c+v_gq+\frac12\beta q^2,\qquad q=k-k_0,\qquad
\beta=\omega''(k_0)=\frac{c^2\omega_0^2}{\omega_c^3}>0.
$$

The distinction between translation and curvature-driven spreading is the same one exposed by the Gaussian pulse calculation in [Pulse Propagation by Richard Fitzpatrick](pulse-propagation-by-richard-fitzpatrick.md) (equations 9.8–9.18). Its first-order approximation is not an assertion that a dispersive packet keeps its shape indefinitely.

Evaluating the quadratic [Gaussian integral](gaussian-integral.md) gives the original approximation

$$
\psi_2(x,t)=\frac{e^{i(k_0x-\omega_ct)}}{\sqrt{1+i\beta t\sigma^2}}
\exp\!\left[-\frac{\sigma^2(x-v_gt)^2}{2(1+i\beta t\sigma^2)}\right],
$$

and hence

$$
|\psi_2(x,t)|=(1+\beta^2t^2\sigma^4)^{-1/4}
\exp\!\left[-\frac{(x-v_gt)^2}{2L(t)^2}\right],\qquad
L(t)=\frac{\sqrt{1+\beta^2t^2\sigma^4}}{\sigma}.
$$

Here $L$ is the amplitude width: the [standard deviation](standard-deviation.md) of the normalized intensity $|\psi_2|^2$ is $L/\sqrt2$. The peak falls as the packet widens, while $\int|\psi_2|^2dx$ stays constant. This conserved integral is not the complete physical [wave energy](wave-energy.md) of the [Klein-Gordon equation](klein-gordon-equation.md).

Rigid translation requires $|\beta|t\sigma^2\ll1$. The quadratic approximation can allow that quantity to be order one, but still requires the accumulated neglected cubic [wave phase](phase-waves.md) to be small over the appreciable spectrum, for example $(t/6)\sup_{|q|\le3\sigma}|\omega'''(k_0+q)|(3\sigma)^3\ll1$. This sufficient check controls only the stated three-width spectral window; the Gaussian tails must also be negligible at the required accuracy. Higher [derivatives](derivative.md) or very long times require returning to the exact spectral integral. The width $L(t)$ is therefore a controlled local approximation; it neither predicts [front velocity](front-velocity.md) nor establishes a universal identity between [group velocity](group-velocity.md) and [information velocity](information-velocity.md).

## ↑ Ancestors (9)

1. [Wave packet](wave-packet.md)
2. [Phase velocity and group velocity](phase-velocity-and-group-velocity.md)
3. [Dispersion relation](dispersion-relation.md)
4. [Wave equation](wave-equation-split.md)
5. [Partial differential equation](partial-differential-equation-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Front velocity](front-velocity.md)
- [Group velocity](group-velocity.md)
- [Wave packet](wave-packet.md)

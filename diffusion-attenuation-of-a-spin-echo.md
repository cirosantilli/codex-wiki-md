# Diffusion attenuation of a spin echo

↑ **Parent:** [Spin echo](spin-echo.md)

A [spin echo](spin-echo.md) refocuses a nucleus's fixed detuning. A nucleus that moves through a [magnetic field gradient](magnetic-field-gradient.md) can have different detunings during the two intervals. To see the distinction without assuming that all [noise](noise-signal-processing.md) is reversible, let $\Delta(t)$ vary during free evolution. With the same pulse convention, its residual [phase](phase-waves.md) at $2\tau$ is

$$
\Phi=\int_0^\tau\Delta(t)\,dt-\int_\tau^{2\tau}\Delta(t)\,dt
=\int_0^{2\tau}y(t)\Delta(t)\,dt,\qquad
y(t)=\begin{cases}+1,&t<\tau,\\-1,&t>\tau.\end{cases}
$$

Static detuning cancels because $\int y(t)\,dt=0$. A detuning $\Delta_a$ during the first interval and $\Delta_b$ during the second leaves $\Phi=\tau(\Delta_a-\Delta_b)$, which need not vanish. The final component [signal](signal.md) is $e^{i\Phi}$ before relaxation; changing the overall receiver convention changes its conjugation but not its magnitude.

For an original quantitative model, take a constant [magnetic field gradient](magnetic-field-gradient.md) $G=dB_z/dx$ and unrestricted one-dimensional [Brownian motion](brownian-motion-split.md) $x(t)=x_0+\sqrt{2D}W_t$, where $D$ is the [diffusion coefficient](diffusion-coefficient.md) and $W_t$ is standard [Brownian motion](brownian-motion-split.md). Then $\Delta(t)=\Delta_0+\gamma Gx(t)$. The constant terms cancel, and the [Gaussian distribution](normal-distribution.md) of the remaining [phase](phase-waves.md) follows from the [Brownian covariance kernel](brownian-covariance-kernel.md) $\mathbb E[W_sW_t]=\min(s,t)$. Writing $Q(r)=\int_r^{2\tau}y(t)\,dt$ gives

$$
Q(r)=\begin{cases}-r,&0\leq r\leq\tau,\\r-2\tau,&\tau\leq r\leq2\tau,\end{cases}\qquad
\operatorname{Var}\Phi=2D\gamma^2G^2\int_0^{2\tau}Q(r)^2\,dr
=\frac43D\gamma^2G^2\tau^3.
$$

The [characteristic function](characteristic-function-split.md) of a zero-mean [Gaussian distribution](normal-distribution.md) now supplies the extra factor $\mathbb E[e^{i\Phi}]=e^{-\operatorname{Var}\Phi/2}$, so

$$
S(2\tau)=\exp\!\left[-\frac{2\tau}{T_2}-\frac23D\gamma^2G^2\tau^3\right].
$$

Here $\gamma$ is in radians per second per tesla, $G$ in tesla per metre, and $D$ in square metres per second: the extra exponent is [dimensionless](dimensionless-quantity.md). The figure chooses $\gamma/(2\pi)=42.58\,\mathrm{MHz/T}$, $G=0.010\,\mathrm{T/m}$ and $D=2.0\times10^{-9}\,\mathrm{m^2/s}$. With the earlier $\tau$ and $T_2$, diffusion reduces the echo from $0.60653$ to about $0.32930$. These are illustrative model parameters, not values extracted from Hahn's experiment.

This result assumes instantaneous perfect pulses, a constant [magnetic field gradient](magnetic-field-gradient.md), unrestricted [diffusion](diffusion.md) with constant [diffusion coefficient](diffusion-coefficient.md), and independent homogeneous [transverse relaxation](transverse-relaxation.md). Restricted motion, changing gradients, finite pulses and interactions between [spins](spin.md) can require different attenuation laws. Even a fixed [Hamiltonian](hamiltonian.md) is refocused only for the terms whose sign the pulse reverses: a simultaneous 180° rotation of two [spins](spin.md) leaves their $J_{z,1}J_{z,2}$ product unchanged, because both factors change sign. A recovered echo therefore demonstrates a particular recoverable phase history, rather than reversal of every microscopic process.

## ↑ Ancestors (4)

1. [Spin echo](spin-echo.md)
2. [Nuclear magnetic resonance](nuclear-magnetic-resonance-split.md)
3. [Chemistry](chemistry-split.md)
4. [Codex Wiki](split.md)

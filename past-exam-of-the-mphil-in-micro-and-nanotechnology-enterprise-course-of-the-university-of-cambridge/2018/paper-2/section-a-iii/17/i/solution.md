<h1 id="section-a-iii/17/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Interpret the given noise correlation as the three-dimensional dot-product correlation. Each Cartesian component then has $\langle\xi_i(t)\xi_j(t')\rangle=2\gamma k_BT\delta_{ij}\delta(t-t')$. For the usual Gaussian thermal-noise idealization, each coordinate is an [Ornstein-Uhlenbeck process](../../../../../../ornstein-uhlenbeck-process.md). With $\tau=\gamma/k$,

$$
\mathbf x(t)=\mathbf x_0e^{-t/\tau}+
\frac1\gamma\int_0^t e^{-(t-s)/\tau}\boldsymbol\xi(s)\,ds.
$$

For a particle initially at $\mathbf x_0=0$,

$$
\langle|\mathbf x(t)|^2\rangle=
\frac{6\gamma k_BT}{\gamma^2}\int_0^t e^{-2(t-s)/\tau}ds
=\frac{3k_BT}{k}(1-e^{-2t/\tau}).
$$

Hence its long-time displacement about the trap/elastic equilibrium has

$$
\boxed{x_{\rm rms}=\sqrt{3k_BT/k}}.
$$

This also follows from [equipartition theorem](../../../../../../equipartition-theorem.md): each of three quadratic coordinates contributes $k_BT/2$.

A different common experimental quantity is the stationary time-lag displacement. It obeys

$$
\langle|\mathbf x(t+\Delta)-\mathbf x(t)|^2\rangle
=\frac{6k_BT}{k}(1-e^{-\Delta/\tau}),
$$

with long-lag RMS $\sqrt{6k_BT/k}$. **The factor of two distinguishes fluctuations about a mean [position](../../../../../../position.md) from differences between two decorrelated [positions](../../../../../../position.md).** The observation convention must be stated rather than silently interchanged.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [17](../../17.md)
3. [Section A(iii)](../../../section-a-iii.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the MPhil in micro- and nanotechnology enterprise course of the University of Cambridge](../../../../../split.md)
7. [MPhil in micro- and nanotechnology enterprise course of the University of Cambridge](../../../../../../mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

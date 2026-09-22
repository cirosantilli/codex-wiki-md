<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define $\Delta t=t-t'$, $\mathbf r=\mathbf x-\mathbf x'$ in the three noncompact spatial directions, and $\Delta w=w-w'$. The compact source must be the periodic [Dirac delta](../../../../../../dirac-delta-function.md)

$$
\delta_R(\Delta w)=\frac1R\sum_{n\in\mathbb Z}e^{ik_n\Delta w},\qquad k_n=\frac{2\pi n}R.
$$

For the wave operator as explicitly defined in the question, a [retarded circle-compactified massless propagator](../../../../../../retarded-circle-compactified-massless-propagator.md) is

$$
\boxed{G_{\mathrm{ret}}=\frac1R\sum_{n\in\mathbb Z}e^{ik_n\Delta w}
\int\frac{d^3k}{(2\pi)^3}\frac{d\omega}{2\pi}
\frac{e^{i\mathbf k\cdot\mathbf r-i\omega\Delta t}}
{\mathbf k^2+k_n^2-(\omega+i0)^2}.}
$$

The poles $\omega=\pm\sqrt{\mathbf k^2+k_n^2}-i0$ are both below the real axis, making the [integral](../../../../../../integral.md) vanish for $\Delta t<0$. Performing just the frequency [integral](../../../../../../integral.md) gives an equivalent expression

$$
G_{\mathrm{ret}}=\frac{\Theta(\Delta t)}R\sum_n e^{ik_n\Delta w}
\int\frac{d^3k}{(2\pi)^3}e^{i\mathbf k\cdot\mathbf r}
\frac{\sin(\Omega_n\Delta t)}{\Omega_n},
\qquad\Omega_n^2=\mathbf k^2+k_n^2.
$$

The first time [derivative](../../../../../../derivative.md) of $\Theta(t)\sin(\Omega t)/\Omega$ jumps by one at zero, so applying $\partial_t^2+\Omega^2$ yields $\delta(t)$. Together with the completeness relations for the [Fourier series](../../../../../../fourier-series-split.md) and [Fourier transform](../../../../../../fourier-transform.md) this verifies the specified source and normalization. The symbol for the wave operator follows the question's explicit sign convention; it is the negative of $g^{AB}\nabla_A\nabla_B$ for its mostly-plus [metric tensor](../../../../../../metric-tensor.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

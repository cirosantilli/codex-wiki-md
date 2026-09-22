<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The real-wavenumber [dispersion relation](../../../../../../dispersion-relation.md) has the explicit branch

$$
\omega(k)=\tfrac12(1-e^{-2ak}),\qquad \omega'(k)=ae^{-2ak}>0\quad(k\in\mathbb R).
$$

Its [frequencies](../../../../../../frequency.md) are real. A real-axis [Fourier transform](../../../../../../fourier-transform.md) propagator multiplies every component by $e^{-i\omega(k)t}$, of modulus one, so a square-integrable localized disturbance has constant $L^2$ norm. For sufficiently smooth localized data with an integrable [Fourier transform](../../../../../../fourier-transform.md), its pointwise [amplitude](../../../../../../wave-amplitude.md) also has a time-independent upper bound. In particular, there is no exponential growth along a fixed or moving ray.

The [Briggs-Bers criterion](../../../../../../briggs-bers-criterion.md) makes the same conclusion while enforcing causality. Start the temporal inversion line at $\operatorname{Im}\omega=\sigma>0$ and the spatial inversion contour on the real $k$ axis. The spatial roots can be followed explicitly:

$$
k_j(\omega)=-\frac{1}{2a}\operatorname{Log}(1-2\omega)+\frac{i\pi j}{a},\qquad j\in\mathbb Z.
$$

Choose the principal logarithm along this upper temporal half-plane. Since $\operatorname{Im}(1-2\omega)<0$, the $j=0$ root lies above the real $k$ axis; the $j=-1$ root lies below it. Successive roots remain separated by $i\pi/a$. As $\sigma$ is lowered, $k_0$ approaches the real axis when $\omega<1/2$ is real. The spatial contour is then indented beneath that root, as required by continuation from positive $\sigma$. No lower root meets it: their separation stays nonzero.

Algebraically,

$$
D_k=-2ae^{-2ak}\ne0
$$

for every finite complex $k$, so there is no finite [spatial pinch point](../../../../../../spatial-pinch-point.md). The logarithmic singularity at $\omega=1/2$ sends roots to $\operatorname{Re}k=+\infty$; it is on the real-frequency boundary, not a positive-growth pinch in the upper temporal half-plane. The continuum of neutral poles is the real curve $\omega<1/2$ in the $\omega$ plane. It is reached as a causal boundary value, rather than producing an upper-half-plane singularity.

The figure follows neighboring spatial roots while lowering horizontal temporal contours. It shows why merely finding roots in both spatial half-planes does not establish an instability: those roots never collide across the inversion contour.

<a id="3/a/image-causal-temporal-contours-and-nonpinching-spatial-roots-of-the-triangular-jet-dispersion-relation"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-74-causal-roots.png)

**[Figure 1](#3/a/image-causal-temporal-contours-and-nonpinching-spatial-roots-of-the-triangular-jet-dispersion-relation). Causal temporal contours and nonpinching spatial roots of the triangular-jet dispersion relation**.

**These modes have neither absolute wave-packet instability nor convective wave-packet instability; they are temporally neutral.** Their positive real [group velocity](../../../../../../group-velocity.md) transports [wave packets](../../../../../../wave-packet.md) downstream. Nonreal spatial roots describe spatial continuation and evanescence, not temporal amplification. The exponential growth criteria concern the causal impulse response, not an unrestricted choice of a complex root.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

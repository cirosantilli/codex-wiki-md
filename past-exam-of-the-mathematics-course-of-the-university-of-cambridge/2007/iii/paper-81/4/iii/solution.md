<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

From part (i), the steady mean has $\coth\Lambda-1/\Lambda=1-1/\Lambda+O(e^{-2\Lambda})$. Hence $BD_r=\Lambda^{-1}\to0$ gives $\mathbf V_c\to V_s\mathbf k$. Part (ii) gives the same mean as $t\to\infty$. Thus

$$
\boxed{\lim_{BD_r\to0}\mathbf V_{c,\mathrm{steady}}
=\lim_{t\to\infty}\mathbf V_{c,D_r=0}(t)=V_s\mathbf k.}
$$

Both limiting distributions concentrate weakly at the upward pole. A common limiting mean does not identify their finite-time distributions or the order in which the limits are taken.

Time scales must be compared at a specified accuracy. The exact deterministic solution approaches the limiting mean with deficit $(4t/B-2)e^{-2t/B}$: its alignment scale is $B$, with exponential late scale $B/2$. For weak but nonzero [diffusion](../../../../../../diffusion.md), linearize about the upward direction using the two transverse tilt components $\mathbf q$. They obey the [Ornstein-Uhlenbeck process](../../../../../../ornstein-uhlenbeck-process.md)

$$
d\mathbf q=-\frac{\mathbf q}{B}dt+\sqrt{2D_r}\,d\mathbf W,
\qquad
\frac{d}{dt}\langle|\mathbf q|^2\rangle=-\frac2B\langle|\mathbf q|^2\rangle+4D_r.
$$

The stationary angular variance is $2BD_r$, and nearby axisymmetric variance perturbations decay on $B/2$ to leading weak-noise order. This is [weak-noise relaxation of gyrotactic alignment](../../../../../../weak-noise-relaxation-of-gyrotactic-alignment.md): the aligning [torque](../../../../../../torque.md), not the pure rotational-diffusion time $D_r^{-1}$, controls the weak-noise alignment rate.

Nevertheless the full relaxation times are not identical. Finite [diffusion](../../../../../../diffusion.md) leaves mean deficit approximately $BD_r$, whereas deterministic alignment has no such floor. Starting from isotropy, reducing the transient deficit to that tiny floor requires $(4t/B-2)e^{-2t/B}\sim BD_r$, or

$$
t\sim\frac B2\log\frac1{BD_r}
$$

with smaller logarithmic corrections. **The two limits have the same mean and the same order-$B$ weak-noise alignment mechanism, but not identical transients or accuracy-dependent settling times.** No finite time achieves the exact deterministic point-mass limit; positive [diffusion](../../../../../../diffusion.md) never gives that exact point mass at all.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 81](../../../paper-81-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

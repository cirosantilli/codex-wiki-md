<h1 id="s3/3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

An [energy measurement](../../../../../energy-measurement.md) selects the [ground state](../../../../../ground-state.md) with [probability](../../../../../probability.md) equal to the squared [inner product](../../../../../inner-product-split.md) with $\psi_1$. Using $N=\sqrt3/L^{3/2}$ and [integration by parts](../../../../../integration-by-parts.md),

$$
c_1=\int_0^L\psi_1(x)^*\Psi(x)\,dx=\frac{\sqrt6}{L^2}\int_0^Lx\sin\frac{\pi x}L\,dx
=\frac{\sqrt6}{\pi}.
$$

Thus

$$
\boxed{\Pr(E=E_1)=|c_1|^2=\frac6{\pi^2}\simeq0.6079.}
$$

The full [Fourier sine series](../../../../../fourier-sine-series.md) has $c_n=(-1)^{n+1}\sqrt6/(n\pi)$, so $\sum_n|c_n|^2=(6/\pi^2)\sum_n n^{-2}=1$, an independent [wavefunction normalization](../../../../../wavefunction-normalization.md) check. However $E_n|c_n|^2=3\hbar^2/(mL^2)$ for every $n$, hence $\sum_nE_n|c_n|^2$ diverges. This explicitly verifies the infinite-[energy expectation](../../../../../energy-expectation.md) qualification in part (b), without invalidating the individual projection [probabilities](../../../../../probability.md).

## ↑ Ancestors (13)

1. [D](../d.md)
2. [3](../../3.md)
3. [S3](../../../s3.md)
4. [2019](../../../../2019-split.md)
5. [Past exam of the short options paper of the physics Prelims of the University of Oxford](../../../../split.md)
6. [Short options paper of the physics Prelims of the University of Oxford](../../../../../short-options-paper-of-the-physics-prelims-of-the-university-of-oxford.md)
7. [Year 1 of the physics course of the University of Oxford](../../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

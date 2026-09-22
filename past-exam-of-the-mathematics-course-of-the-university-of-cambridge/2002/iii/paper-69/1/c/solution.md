<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Each nonzero mode is Gaussian, giving the [covariance](../../../../../../covariance.md)

$$
\langle h_{\mathbf q}h_{\mathbf q'}\rangle=\frac{k_BT}{\sigma q^2}(2\pi)^D\delta^{(D)}(\mathbf q+\mathbf q').
$$

Consequently the [capillary height-difference correlation](../../../../../../capillary-height-difference-correlation.md) is

$$
\boxed{B(r)=\langle[h(\mathbf r)-h(0)]^2\rangle
=\frac{2k_BT}{\sigma}\int_{\mathbf q}\frac{1-\cos(\mathbf q\cdot\mathbf r)}{q^2}.}
$$

The difference removes the zero mode and makes the integral infrared-finite at each fixed separation. Where required, cut off $q$ at $\Lambda\sim1/a$ with microscopic length $a$. The question's $d$ is the embedding dimension, so the momentum integral has dimension $D=d-1$, not $d$.

For $d=2$, $D=1$, use $\int_{-\infty}^{\infty}dq\,(1-\cos qr)/(2\pi q^2)=|r|/2$. Hence

$$
\boxed{B(r)=\frac{k_BT}{\sigma}|r|\quad(d=2).}
$$

The root-mean-square relative height grows as $r^{1/2}$: the interface wanders increasingly far from a fixed height.

For $d=3$, $D=2$, angular integration gives

$$
B(r)=\frac{k_BT}{\pi\sigma}\int_0^\Lambda\frac{dq}{q}[1-J_0(qr)]
=\frac{k_BT}{\pi\sigma}\log(r/a)+O(k_BT/\sigma),\qquad r\gg a.
$$

The [Bessel function](../../../../../../bessel-function.md) expression separates the universal logarithmic growth from a cutoff-dependent constant. The membrane is logarithmically rough, so its absolute height fluctuations are unbounded in the [thermodynamic limit](../../../../../../thermodynamic-limit.md) even though long-wavelength slopes need not be large.

For $d=4$, $D=3$, the massless Green function at nonzero separation is $1/(4\pi r)$. Thus

$$
\boxed{B(r)=B_\infty-\frac{k_BT}{2\pi\sigma r}+o(r^{-1})\quad(d=4),}
$$

where $B_\infty$ is finite once the microscopic cutoff is supplied. For a spherical sharp cutoff, $B_\infty=k_BT\Lambda/(\pi^2\sigma)$. Relative height fluctuations saturate at large distance, allowing a localized interface height selected by boundaries. **The roughness distinction is linear growth in $d=2$, logarithmic growth in $d=3$, and bounded long-distance fluctuations in $d=4$.** The short-distance cutoff and the small-slope assumption remain necessary; bounded height fluctuations do not imply a perfectly flat microscopic membrane.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

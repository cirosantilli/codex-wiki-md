<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

To match the positive source printed in the question, choose [synchronous gauge](../../../../../../synchronous-gauge-in-cosmology.md) metric

$$
ds^2=a^2\left[-d\tau^2+(\delta_{ij}-h_{ij})dx^idx^j\right].
$$

The commonly used convention with $\delta_{ij}+h_{ij}$ gives the opposite source sign; switching conventions means replacing $h$ and $h_S$ by their negatives together. This distinction is necessary when comparing with the usual [synchronous photon brightness equation](../../../../../../synchronous-photon-brightness-equation.md).

Let $p^\alpha=dx^\alpha/d\lambda$ be the photon tangent for an affine parameter. The covariant [geodesic equation](../../../../../../geodesic-equation.md) is

$$
\frac{d\widetilde p_\nu}{d\lambda}=\frac12g_{\alpha\beta,\nu}p^\alpha p^\beta.
$$

For $\nu=0$, the homogeneous scale-factor contributions cancel by the [null geodesic](../../../../../../null-geodesic.md) condition, leaving $d\widetilde p_0/d\lambda=-a^2h'_{ij}p^ip^j/2$. Since $\widetilde p_0=-a^2p^0=-q$ and $d\tau/d\lambda=p^0$, use the background $p^i=p^0n^i$ in this first-order term to obtain

$$
\boxed{q'=\frac12q h'_{ij}n^in^j.}
$$

Using the affine form also avoids confusing a covariant $p_0$ with the contravariant factor $p^0$ required when changing the geodesic parameter to coordinate time.

In [conformal time](../../../../../../conformal-time.md), the equation from part(a) becomes $f_1'+n^i\partial_i f_1+q'f_0'=0$. A Fourier mode proportional to $e^{i\mathbf k\cdot\mathbf x}$ has streaming term $ik\mu f_1$. Multiply by $-4/(qf_0')$; its prefactor is background-time independent. With $\Delta=-4f_1/(qf_0')$,

$$
\Delta'+ik\mu\Delta=4q'/q=2h'_{ij}n^in^j.
$$

Contracting the scalar decomposition explicitly gives

$$
h'_{ij}n^in^j=\frac{h'}3+\left(\mu^2-\frac13\right)h_S',
$$

so

$$
\boxed{\Delta'+ik\mu\Delta=\frac23(h'-h_S')+2\mu^2h_S'.}
$$

This is the [photon brightness equation for a negative spatial perturbation](../../../../../../photon-brightness-equation-for-a-negative-spatial-perturbation.md). For a perturbation of blackbody-temperature form, $f_1=-qf_0'\Theta$, so $\Delta=4\Theta$ is the [photon brightness perturbation](../../../../../../photon-brightness-perturbation.md). A more general initial spectral distortion can retain $q$ dependence; the gravitational forcing is still independent of $q$ in this linear massless equation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

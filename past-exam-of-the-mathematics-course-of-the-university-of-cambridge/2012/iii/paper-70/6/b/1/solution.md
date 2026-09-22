<h1 id="6/b/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the printed [Fourier transform](../../../../../../../fourier-transform.md) convention $\widehat\phi(t)=\int\phi(x)e^{-ixt}\,dx$, interpreted by the [Plancherel theorem](../../../../../../../plancherel-theorem.md) when $\phi$ is only square integrable. By the scaling and [function translation](../../../../../../../translation-of-a-function.md) rules,

$$
\widehat{\phi(2\cdot-n)}(t)=\frac12e^{-int/2}f(t/2).
$$

Taking the [Fourier transform](../../../../../../../fourier-transform.md) of the [scaling refinement equation](../../../../../../../scaling-refinement-equation.md) gives $f(t)=m(t/2)f(t/2)$, or equivalently

$$
\boxed{f(2t)=m(t)f(t),\qquad m(t)=\frac12\sum_na_ne^{-int}.}
$$

Conversely this identity, the same scaling rule and injectivity of the [Fourier transform](../../../../../../../fourier-transform.md) recover the [scaling refinement equation](../../../../../../../scaling-refinement-equation.md).

For infinite filters, these statements are equalities in $L^2$, with [Fourier series](../../../../../../../fourier-series-split.md) understood in $L^2[0,2\pi]$. Under the accompanying [orthonormality](../../../../../../../orthonormal-set.md) condition, $\{\sqrt2\phi(2\cdot-n)\}$ is an [orthonormal sequence](../../../../../../../orthonormal-sequence.md), so the refinement series converges in $L^2$ precisely for $a\in\ell^2$. Moreover the condition in part (b)(2) makes multiplication by $f$ an [isometry](../../../../../../../isometry.md) from periodic $L^2$ symbols into $L^2(\mathbb R)$:

$$
\int_{\mathbb R}|m(t)f(t)|^2\,dt=\int_0^{2\pi}|m(t)|^2\sum_k|f(t+2\pi k)|^2\,dt=\int_0^{2\pi}|m(t)|^2\,dt.
$$

Applying this to finite filter truncations justifies passage to the limit in both directions. Thus the two paired assertions have a rigorous equivalent interpretation without requiring absolute integrability of $\phi$.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Paper 70](../../../../paper-70-split.md)
5. [Iii](../../../../split.md)
6. [2012](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

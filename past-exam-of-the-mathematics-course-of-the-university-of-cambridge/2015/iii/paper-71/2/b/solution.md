<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Hilbert-transform Fourier multiplier](../../../../../../hilbert-transform-fourier-multiplier.md) is bounded, and $\xi^r\widehat\varphi(\xi)$ is integrable for every nonnegative integer $r$. Therefore its inverse [Fourier transform](../../../../../../fourier-transform.md) can be differentiated under the integral arbitrarily many times:

$$
\partial_x^r\mathcal H\varphi(x)=\frac1{2\pi}\int e^{ix\xi}(i\xi)^r[-i\operatorname{sgn}(\xi)]\widehat\varphi(\xi)\,d\xi.
$$

These [derivatives](../../../../../../derivative.md) are continuous by [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md). Since $\widehat{\varphi^{(r)}}=(i\xi)^r\widehat\varphi$, **the Hilbert transform is smooth and commutes with differentiation**:

$$
\boxed{\mathcal H\varphi\in C^\infty(\mathbb R),\qquad (\mathcal H\varphi)'=\mathcal H(\varphi').}
$$

The Fourier proof avoids differentiating a singular kernel without preserving its [Cauchy principal value](../../../../../../cauchy-principal-value.md) prescription.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="24j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First $\int_{\mathbb R}e^{-x^2/2}\,dx=\sqrt{2\pi}$: square the positive [integral](../../../../../../integral.md) and use polar coordinates to obtain $2\pi\int_0^\infty re^{-r^2/2}\,dr=2\pi$. Scaling therefore normalizes the one-dimensional [Gaussian function](../../../../../../gaussian-function.md) $g_t$.

Let $I(\xi)=\int_{\mathbb R}(2\pi t)^{-1/2}e^{-x^2/(2t)}e^{-i\xi x}\,dx$. Differentiation under the [integral](../../../../../../integral.md) is justified by the integrable majorant $|x|g_t(x)$. Since $g_t'(x)=-xg_t(x)/t$, [integration by parts](../../../../../../integration-by-parts.md), with zero endpoint terms, gives $I'(\xi)=-t\xi I(\xi)$. With $I(0)=1$, this yields $I(\xi)=e^{-t\xi^2/2}$. Multiplication of the one-dimensional [integrals](../../../../../../integral.md) gives

$$
\boxed{\widehat g_t(\xi)=e^{-t|\xi|^2/2}.}
$$

Applying the same computation with reciprocal scale $1/t$ evaluates its inverse [integral](../../../../../../integral.md):

$$
(2\pi)^{-d}\int e^{i\xi\cdot x}e^{-t|\xi|^2/2}\,d\xi
=(2\pi t)^{-d/2}e^{-|x|^2/(2t)}=g_t(x).
$$

For $f\in L^1$, [Fubini's theorem](../../../../../../fubini-s-theorem.md) gives $\widehat{f*g_t}=\widehat f\,e^{-t|\xi|^2/2}$, which is integrable because $\widehat f$ is bounded. Its inverse [integral](../../../../../../integral.md) is

$$
\int_{\mathbb R^d} f(y)\left[(2\pi)^{-d}\int_{\mathbb R^d}e^{i\xi\cdot(x-y)}e^{-t|\xi|^2/2}\,d\xi\right]dy
=\int f(y)g_t(x-y)\,dy.
$$

Absolute integrability of $|f(y)|e^{-t|\xi|^2/2}$ justifies this second application of [Fubini's theorem](../../../../../../fubini-s-theorem.md). Thus **[Fourier inversion](../../../../../../fourier-inversion-theorem.md) holds for every Gaussian [convolution](../../../../../../convolution.md)**, in fact pointwise for this [continuous](../../../../../../continuous-function.md) representative.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [24J](../../24j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

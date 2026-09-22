<h1 id="5a/solution">Solution</h1>

↑ **Parent:** [5A](../5a.md)

Use the [Fourier transform](../../../../../fourier-transform.md) convention

$$
\widehat f(s)=\int_{\mathbb R}f(x)e^{isx}dx,\qquad
f(x)=\frac1{2\pi}\int_{\mathbb R}\widehat f(s)e^{-isx}ds.
$$

This convention also gives the sign of the inverse transform in 15A. The [Parseval identity](../../../../../parseval-identity.md), in its bilinear form, is

$$
\boxed{\int_{\mathbb R}f(x)\overline{g(x)}dx
=\frac1{2\pi}\int_{\mathbb R}\widehat f(s)\overline{\widehat g(s)}ds.}
$$

In particular $\int|f|^2=(2\pi)^{-1}\int|\widehat f|^2$. Initially take $f,g$ to be [Schwartz functions](../../../../../schwartz-function.md); the formula then extends to $L^2$ with Fourier transforms interpreted by completion.

Here is a proof which also justifies the needed limit operations. For $\varepsilon>0$, form

$$
I_\varepsilon=\frac1{2\pi}\int\widehat f(s)\overline{\widehat g(s)}e^{-\varepsilon s^2}ds.
$$

Absolute integrability allows [Fubini's theorem](../../../../../fubini-s-theorem.md) to replace the transformed factors by their defining integrals. The elementary Gaussian integral gives

$$
K_\varepsilon(t)=\frac1{2\pi}\int e^{ist-\varepsilon s^2}ds
=\frac1{\sqrt{4\pi\varepsilon}}e^{-t^2/(4\varepsilon)},
$$

so $I_\varepsilon=\int f(x)\overline{(K_\varepsilon*g)(x)}dx$, with [convolution](../../../../../convolution.md) $(h*g)(x)=\int h(x-y)g(y)dy$. The kernel is nonnegative, has integral one, and its mass outside any fixed neighborhood of zero tends to zero. Since a Schwartz function is bounded and uniformly continuous, splitting the convolution difference into small and large $|x-y|$ proves $K_\varepsilon*g\to g$ uniformly. As $f\in L^1$, the last integral consequently tends to $\int f\overline g$.

On the spectral side, repeated [integration by parts](../../../../../integration-by-parts.md) makes the transforms rapidly decreasing; their product is integrable. The [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) therefore gives $I_\varepsilon\to(2\pi)^{-1}\int\widehat f\overline{\widehat g}$. Equating the two limits proves the displayed identity. For general $L^2$ functions, approximate by Schwartz functions. The norm identity makes their transforms Cauchy in $L^2$ with the prescribed factor; the limit defines the $L^2$ Fourier transform independently of the approximation. Taking limits in the bilinear identity proves it for all $L^2$ pairs. Thus the proof includes the hypotheses and avoids unjustified exchanges of nonabsolutely convergent integrals.

## ↑ Ancestors (10)

1. [5A](../5a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

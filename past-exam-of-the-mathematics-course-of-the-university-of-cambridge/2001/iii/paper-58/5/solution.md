<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The original PDF's kernel has an incorrect normalization. With ordinary $dt$, its integral is $\pi$, not one. Already at $n=1$ the printed kernel is the constant $1/2$. For $f\equiv1$, the printed operator therefore returns $\pi$, while $\omega(f,\delta)=0$ for every $\delta$. Thus **the literal inequality with the printed kernel is false**. The [Fejér kernel](../../../../../fejer-kernel.md) representing the stated average of [Fourier partial sums](../../../../../fourier-partial-sum.md) is

$$
K_n(t)=\frac1{2\pi n}\left(\frac{\sin(nt/2)}{\sin(t/2)}\right)^2,
\qquad \int_{-\pi}^{\pi}K_n(t)\,dt=1.
$$

The ratio at zero is interpreted by its limit. To verify the normalization and the averaging property, use the finite geometric sum:

$$
K_n(t)=\frac1{2\pi n}\left|\sum_{j=0}^{n-1}e^{ijt}\right|^2
=\frac1{2\pi}\sum_{|r|<n}\left(1-\frac{|r|}{n}\right)e^{irt}.
$$

[Fourier orthogonality](../../../../../fourier-orthogonality.md) gives unit integral; the displayed [Fourier coefficients](../../../../../fourier-coefficient.md) are exactly the multipliers of the [Fejér sum](../../../../../fejer-sum.md). This also proves nonnegativity.

For the correctly normalized [Fejér sum](../../../../../fejer-sum.md), subtraction of $f(x)$ gives

$$
|\sigma_{n-1}f(x)-f(x)|\le\int_{-\pi}^{\pi}K_n(t)|f(x-t)-f(x)|\,dt.
$$

Take $0<\delta\le1$ and split at $|t|=\delta$. The inner part is at most $\omega(f,\delta)$, because the kernel is nonnegative and has mass one. The strict inequality in the definition of the [modulus of continuity](../../../../../modulus-of-continuity.md) causes no endpoint issue: [continuity](../../../../../continuous-function.md) gives the same bound at distance exactly $\delta$.

On $0<|t|\le\pi$, $\sin(|t|/2)\ge|t|/\pi$, so

$$
K_n(t)\le\frac{\pi}{2nt^2},\qquad\int_{\delta\le|t|\le\pi}K_n(t)\,dt\le\frac{\pi}{n\delta}.
$$

Divide an arc of length $|t|$ into at most $1+|t|/\delta$ shorter arcs. The [triangle inequality](../../../../../triangle-inequality.md) then bounds $|f(x-t)-f(x)|$ by $(1+\pi/\delta)\omega(f,\delta)$. Consequently

$$
\|\sigma_{n-1}f-f\|_\infty\le\left[1+\frac{\pi}{n\delta}\left(1+\frac\pi\delta\right)\right]\omega(f,\delta).
$$

Choosing $\delta=n^{-1/2}$ proves the requested [fractional-scale Fejér approximation bound](../../../../../fractional-scale-fejer-approximation-bound.md) for the intended normalization, for example with the absolute constant $1+\pi+\pi^2$:

$$
\boxed{\|\sigma_{n-1}f-f\|_\infty\le(1+\pi+\pi^2)\,\omega(f,n^{-1/2}).}
$$

The same proof applies to complex-valued [continuous functions](../../../../../continuous-function.md), since the estimates use absolute values.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 58](../../paper-58-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

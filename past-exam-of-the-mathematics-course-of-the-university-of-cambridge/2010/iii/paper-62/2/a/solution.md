<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the centered [second modulus of smoothness](../../../../../../second-modulus-of-smoothness.md)

$$
\omega_2(f,\delta)=\sup_{|h|\le\delta}\|f(\cdot+h)-2f+f(\cdot-h)\|_\infty.
$$

The relevant modulus properties are $\omega_2(f,t)\le(1+t/\delta)^2\omega_2(f,\delta)$ for $t\ge0$, $\delta>0$, and $\omega_2(f,\delta)\le\delta^2\|f''\|_\infty$ when $f''$ is continuous. The latter follows from the [second-difference integral formula](../../../../../../second-difference-integral-formula.md)

$$
f(x+h)-2f(x)+f(x-h)=\int_{-|h|}^{|h|}(|h|-|u|)f''(x+u)\,du.
$$

The [Fejér kernel](../../../../../../fejer-kernel.md) is even, nonnegative and has integral one. Averaging the convolution at $t$ and $-t$ therefore gives

$$
\sigma_nf(x)-f(x)=\frac12\int_{-\pi}^{\pi}F_n(t)\bigl(f(x+t)-2f(x)+f(x-t)\bigr)\,dt.
$$

Apply the [second modulus of smoothness](../../../../../../second-modulus-of-smoothness.md) bound and $(1+s)^2\le2(1+s^2)$:

$$
\|\sigma_nf-f\|_\infty\le\omega_2(f,\delta)\left(1+\delta^{-2}\int_{-\pi}^{\pi}t^2F_n(t)\,dt\right).
$$

For $|t|\le\pi$, $\sin(|t|/2)\ge|t|/\pi$, while $\sin^2(nt/2)\le1$. Thus

$$
t^2F_n(t)\le\frac{\pi}{2n},\qquad \int_{-\pi}^{\pi}t^2F_n(t)\,dt\le\frac{\pi^2}{n}.
$$

The removable value at $t=0$ causes no problem. With $\delta=n^{-1/2}$, the [Fejér second-modulus approximation bound](../../../../../../fejer-second-modulus-approximation-bound.md) is

$$
\boxed{\|\sigma_nf-f\|_\infty\le(1+\pi^2)\omega_2(f,n^{-1/2}).}
$$

If $f''$ is continuous, this also yields **$\|\sigma_nf-f\|_\infty\le(1+\pi^2)\|f''\|_\infty/n=O(n^{-1})$**.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

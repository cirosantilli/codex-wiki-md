<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Use the central second difference $\Delta_t^2f(x)=f(x+t)-2f(x)+f(x-t)$ and define the [second modulus of smoothness](../../../../../second-modulus-of-smoothness.md) by

$$
\omega_2(f,\delta)=\sup_{|h|\le\delta}\|\Delta_h^2f\|_\infty.
$$

We first need its scaling inequality. If $q$ is a positive [integer](../../../../../integer.md), translation by $h$ gives the telescoping identity

$$
\Delta_{qh}^2f(x)=\sum_{j=-q+1}^{q-1}(q-|j|)\Delta_h^2f(x+jh).
$$

The weights sum to $q^2$. For $t>0$, choose $q=\lceil t/\delta\rceil$ and $h=t/q\le\delta$; then

$$
\omega_2(f,t)\le\left(1+\frac t\delta\right)^2\omega_2(f,\delta).
$$

The same bound covers $t=0$ trivially.

In the paper's normalization, the [Fejér kernel](../../../../../fejer-kernel.md) is even and nonnegative, with $\pi^{-1}\int_{-\pi}^{\pi}F_n=1$. Pairing the positive and negative translations expresses the [Fejér sum](../../../../../fejer-sum.md) error as

$$
\sigma_nf(x)-f(x)=\frac1{2\pi}\int_{-\pi}^{\pi}F_n(t)\Delta_t^2f(x)\,dt.
$$

Use the scaling bound and $(1+s)^2\le2(1+s^2)$ to obtain

$$
\|\sigma_nf-f\|_\infty
\le\omega_2(f,\delta)\left[1+\frac1{\pi\delta^2}
\int_{-\pi}^{\pi}t^2F_n(t)\,dt\right].
$$

For $|t|\le\pi$, $\sin(|t|/2)\ge|t|/\pi$. Bounding the numerator sine by one gives

$$
t^2F_n(t)\le\frac{\pi^2}{2n},\qquad
\frac1\pi\int_{-\pi}^{\pi}t^2F_n(t)\,dt\le\frac{\pi^2}{n}.
$$

The bound at $t=0$ holds by continuity. Choosing $\delta=n^{-1/2}$ proves the [Fejér second-modulus approximation bound](../../../../../fejer-second-modulus-approximation-bound.md) with an explicit universal constant:

$$
\boxed{\|\sigma_nf-f\|_\infty\le(1+\pi^2)\omega_2(f,n^{-1/2}).}
$$

Finally, for twice continuously differentiable periodic $f$, two applications of the [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md) give the [second-difference integral formula](../../../../../second-difference-integral-formula.md)

$$
\Delta_h^2f(x)=\int_{-|h|}^{|h|}(|h|-|v|)f''(x+v)\,dv.
$$

The triangular weight has integral $h^2$, so $\omega_2(f,\delta)\le\delta^2\|f''\|_\infty$. Therefore

$$
\boxed{\|\sigma_nf-f\|_\infty\le\frac{(1+\pi^2)\|f''\|_\infty}{n}
=O(n^{-1}).}
$$

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 71](../../paper-71-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

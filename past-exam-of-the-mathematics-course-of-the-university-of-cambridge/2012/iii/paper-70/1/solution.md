<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $\Delta_t^2f(x)=f(x+t)-2f(x)+f(x-t)$, and use the [second modulus of smoothness](../../../../../second-modulus-of-smoothness.md) $\omega_2(f,h)=\sup_{|t|\le h}\|\Delta_t^2f\|_\infty$. The [Jackson kernel](../../../../../jackson-kernel.md) is even, nonnegative and has unit integral. Pairing the two halves of its [convolution](../../../../../convolution.md) therefore gives

$$
j_nf(x)-f(x)=\frac12\int_{-\pi}^{\pi}\Delta_t^2f(x)J_n(t)\,dt.
$$

We need a weighted moment estimate rather than just concentration of the [Jackson kernel](../../../../../jackson-kernel.md). For $|t|\le\pi$, the bounds $|\sin(t/2)|\ge |t|/\pi$ and $|\sin(nt/2)|\le\min(n|\sin(t/2)|,1)$ imply

$$
0\le J_n(t)\le C\min\{n,n^{-3}|t|^{-4}\}.
$$

Consequently, splitting the integral at $1/n$ gives

$$
\int_{-\pi}^{\pi}t^2J_n(t)\,dt
\le 2C\left(n\int_0^{1/n}t^2\,dt+n^{-3}\int_{1/n}^{\pi}t^{-2}\,dt\right)\le C'n^{-2}.
$$

The [second modulus of smoothness](../../../../../second-modulus-of-smoothness.md) satisfies $\omega_2(f,t)\le(1+t/h)^2\omega_2(f,h)$ for $t\ge0$. To see this, choose $q=\lceil t/h\rceil$ when $t>0$, put $u=t/q$, and factor the [function translation](../../../../../translation-of-a-function.md) difference $T_t-I=(T_u-I)\sum_{r=0}^{q-1}T_u^r$. Squaring gives at most $q^2$ translated second differences of step $u$. Each [function translation](../../../../../translation-of-a-function.md) is an [isometry](../../../../../isometry.md) in the [supremum norm](../../../../../supremum-norm.md), and centered and forward second differences have the same [supremum norm](../../../../../supremum-norm.md). This proves the stated scaling bound.

Taking $h=1/n$, using $(1+n|t|)^2\le2+2n^2t^2$, and integrating against the [Jackson kernel](../../../../../jackson-kernel.md) now proves

$$
\|j_nf-f\|_\infty\le\frac12\omega_2(f,1/n)\int_{-\pi}^{\pi}(1+n|t|)^2J_n(t)\,dt\le C''\omega_2(f,1/n).
$$

Thus **the Jackson operator estimate is uniform in both $f$ and $n$**.

For the requested degree-$n$ [best uniform approximation](../../../../../best-uniform-approximation.md), note that the [Jackson kernel](../../../../../jackson-kernel.md), and hence $j_mf$, has [trigonometric polynomial](../../../../../trigonometric-polynomial.md) degree at most $2(m-1)$. Indeed the fourth power in the [Jackson kernel](../../../../../jackson-kernel.md) is the squared modulus of a squared sum of $m$ consecutive complex exponentials. Choose $m=\lfloor n/2\rfloor+1$, so $2(m-1)\le n$ and $m\ge n/2$. The [second-difference integral formula](../../../../../second-difference-integral-formula.md) gives

$$
\Delta_t^2f(x)=\int_{-|t|}^{|t|}(|t|-|u|)f''(x+u)\,du,
\qquad \omega_2(f,h)\le h^2\|f''\|_\infty.
$$

Applying the [Jackson operator estimate](../../../../../jackson-operator-estimate.md) with this $m$ yields the concise answer

$$
\boxed{E_n(f)\le \|j_mf-f\|_\infty\le \frac{4C''}{n^2}\|f''\|_\infty\quad(n\ge1).}
$$

The change of index is essential: $j_nf$ itself generally has degree $2n-2$, exceeding the permitted degree.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 70](../../paper-70-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

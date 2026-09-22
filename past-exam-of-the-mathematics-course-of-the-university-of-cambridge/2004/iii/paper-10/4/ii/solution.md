<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

First establish the norm estimate behind the [spectral-radius three-circle inequality](../../../../../../spectral-radius-three-circle-inequality.md). If $g$ is a holomorphic [Banach space](../../../../../../banach-space-split.md)-valued function on a neighborhood of an annulus $r_0\leq|z|\leq r_1$, then for $r_0<r<r_1$ and $\theta=\log(r/r_0)/\log(r_1/r_0)$,

$$
\sup_{|z|=r}\|g(z)\|\leq\left(\sup_{|z|=r_0}\|g(z)\|\right)^{1-\theta}\left(\sup_{|z|=r_1}\|g(z)\|\right)^\theta.
$$

Here is the underlying [Hadamard three-circle theorem](../../../../../../hadamard-three-circle-theorem.md) argument. For any bounded linear functional $\ell$ of norm at most one, $\ell(g)$ is scalar holomorphic. Its logarithmic modulus is [subharmonic](../../../../../../subharmonic-function.md). Compare it on the annulus with the harmonic function affine in $\log|z|$ whose boundary values are the logarithms of the two boundary norm bounds. The [maximum principle for subharmonic functions](../../../../../../maximum-principle-for-subharmonic-functions.md) gives the interpolated bound inside. Using slightly larger positive bounds and then taking limits handles zeros. The [Hahn-Banach theorem](../../../../../../hahn-banach-theorem.md) identifies the norm with the supremum over these scalar functionals, proving the displayed Banach-valued estimate.

Apply this estimate to $g(z)=f(z)^{2^n}$ and take the $2^n$-th root. On either boundary circle the nonnegative continuous functions

$$
q_n(z)=\|f(z)^{2^n}\|^{1/2^n}
$$

decrease, because submultiplicativity gives $q_{n+1}\leq q_n$. The [spectral radius formula](../../../../../../spectral-radius-formula.md) gives their pointwise limit $r(f(z))$. Part (i) passes their boundary suprema to the limit. With $M_r=\sup_{|z|=r}r(f(z))$ we obtain the general estimate

$$
M_r\leq M_{r_0}^{1-\theta}M_{r_1}^{\theta}.
$$

In particular, take $r_0=R^{-1}$, $r=1$, $r_1=R$, so $\theta=1/2$. Since $r(f(1))\leq M_1$,

$$
\boxed{r(f(1))^2\leq\left(\sup_{|z|=R}r(f(z))\right)\left(\sup_{|z|=R^{-1}}r(f(z))\right).}
$$

This proves the requested inequality without assuming continuity of the spectral radius on the circles.

For the final [spectral-radius Liouville theorem](../../../../../../spectral-radius-liouville-theorem.md), suppose $r(f(z))\leq C$ on the whole plane. The case $C=0$ is immediate. Center circles at an arbitrary $a$, and put $M_a(t)=\sup_{|z-a|=t}r(f(z))$. For $0<\delta<r<R$, the same argument gives

$$
M_a(r)\leq M_a(\delta)^{\log(R/r)/\log(R/\delta)}C^{\log(r/\delta)/\log(R/\delta)}.
$$

If $M_a(\delta)=0$, this forces $M_a(r)=0$. Otherwise let $R\to\infty$ to get $M_a(r)\leq M_a(\delta)$. Upper semicontinuity, proved in 2(a), gives $M_a(\delta)\leq r(f(a))+\varepsilon$ for all sufficiently small $\delta$. Thus every $z$ satisfies $r(f(z))\leq r(f(a))$. The center $a$ is arbitrary, so reversing the two points gives equality. Hence **the spectral radius is constant**. The algebra-valued function itself need not be constant; $f(z)=zN$ with a nonzero square-zero matrix $N$ is a useful example.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 10](../../../paper-10-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

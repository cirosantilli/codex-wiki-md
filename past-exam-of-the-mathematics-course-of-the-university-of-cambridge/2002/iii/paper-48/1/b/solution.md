<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The phase $f(x)=x(1-\cos x)$ is nonnegative on the interval and vanishes only at its two endpoints. An interval away from both endpoints contributes exponentially little, so both endpoint contributions must be expanded before their orders are ranked.

At the left endpoint,

$$
f(x)=\frac{x^3}{2}-\frac{x^5}{24}+O(x^7).
$$

The [Laplace's method](../../../../../../laplace-s-method.md) scale is $x=\sigma^{-1/3}z$. Hence its leading contribution is

$$
\sigma^{-1/3}\int_0^\infty e^{-z^3/2}\,dz
=\frac{2^{1/3}}3\Gamma\left(\frac13\right)\sigma^{-1/3}.
$$

The substitution $v=z^3/2$ evaluates the [integral](../../../../../../integral.md) by the [Gamma function](../../../../../../gamma-function.md). Since there is no quartic term in the phase, the next left-end correction is relatively $O(\sigma^{-2/3})$, and thus absolutely $O(\sigma^{-1})$.

At the right endpoint put $r=2\pi-x$. There

$$
f(2\pi-r)=\pi r^2-\frac{r^3}{2}+O(r^4),
$$

so $r=\sigma^{-1/2}z$ gives

$$
\sigma^{-1/2}\int_0^\infty e^{-\pi z^2}\,dz
=\frac12\sigma^{-1/2}.
$$

The leading right-end integral is a [Gaussian integral](../../../../../../gaussian-integral.md). Its first correction is also absolutely $O(\sigma^{-1})$. The [mixed cubic and quadratic Laplace endpoints](../../../../../../mixed-cubic-and-quadratic-laplace-endpoints.md) therefore produce the first two global terms

$$
\boxed{\mathcal I(\sigma)=
\frac{2^{1/3}\Gamma(1/3)}{3\sigma^{1/3}}
+\frac1{2\sigma^{1/2}}+O(\sigma^{-1})}.
$$

Keeping only the dominant cubic endpoint would miss the second term, which is larger than that endpoint's own first correction.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

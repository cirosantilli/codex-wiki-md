<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Fejér kernel](../../../../../../fejer-kernel.md) is nonnegative, and preservation of constants gives

$$
\boxed{\pi^{-1}\int_{\mathbb T}|F_n(t)|dt=1}.
$$

By evenness,

$$
\sigma_n(f,x)-f(x)=\frac1{2\pi}\int_{\mathbb T}F_n(t)[f(x-t)-2f(x)+f(x+t)]dt.
$$

Put $\delta=n^{-1/2}$. Use $\omega_2(f,|t|)\leq(|t|/\delta+1)^2\omega_2(f,\delta)$ together with $F_n(t)\leq n/2$ and $F_n(t)\leq C/(nt^2)$. Splitting at $1/n$ and $\delta$ shows that the remaining weighted integral is uniformly bounded, so

$$
\boxed{\lVert\sigma_n(f)-f\rVert_\infty\leq C\omega_2(f,n^{-1/2})}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 318](../../../paper-318-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

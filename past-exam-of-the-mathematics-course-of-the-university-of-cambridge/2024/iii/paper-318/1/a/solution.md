<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Averaging the integral representations of the [Fourier partial sums](../../../../../../fourier-partial-sum.md) gives

$$
\sigma_n(f,x)=\frac1\pi\int_{\mathbb T}
\left(\frac1n\sum_{k=0}^{n-1}D_k(x-t)\right)f(t)\,dt.
$$

The finite trigonometric sum is

$$
\sum_{k=0}^{n-1}\sin\left(k+\frac12\right)u
=\frac{\sin^2(nu/2)}{\sin(u/2)}.
$$

Since $D_k(u)=\sin((k+1/2)u)/(2\sin(u/2))$, the [Fejér kernel](../../../../../../fejer-kernel.md) is therefore

$$
\boxed{F_n(u)=\frac1n\sum_{k=0}^{n-1}D_k(u)
=\frac1{2n}\frac{\sin^2(nu/2)}{\sin^2(u/2)}}
$$

and

$$
\boxed{\sigma_n(f,x)=\frac1\pi
\int_{\mathbb T}F_n(x-t)f(t)\,dt}.
$$

The displayed square shows that $F_n\geq0$. Every [Fourier partial sum](../../../../../../fourier-partial-sum.md) preserves the constant function, so $\sigma_n(1)=1$. Substituting $f=1$ in the integral formula gives

$$
\frac1\pi\int_{\mathbb T}F_n(t)\,dt=1.
$$

Nonnegativity then yields

$$
\boxed{\frac1\pi\int_{\mathbb T}|F_n(t)|\,dt=1}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 318](../../../paper-318-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

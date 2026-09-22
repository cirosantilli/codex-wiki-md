<h1 id="19c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [probabilists' Hermite polynomials](../../../../../../probabilists-hermite-polynomial.md) satisfy

$$
\mathrm{He}'_n=n\mathrm{He}_{n-1},
\qquad
x\mathrm{He}_n=\mathrm{He}_{n+1}+n\mathrm{He}_{n-1},
$$

which follow by differentiating the Rodrigues formula. Thus

$$
\boxed{\mathrm{He}_{n+1}=x\mathrm{He}_n-n\mathrm{He}_{n-1}},
$$

so $\alpha_n=0$ and $\beta_n=n$.

For the squared norm, substitute the Rodrigues formula and integrate by parts $n$ times. All boundary terms vanish under the Gaussian weight, and $\mathrm{He}_n^{(n)}=n!$, giving

$$
\begin{aligned}
\langle\mathrm{He}_n,\mathrm{He}_n\rangle
&=(-1)^n\int_{-\infty}^{\infty}
\mathrm{He}_n(x)\frac{d^n}{dx^n}e^{-x^2/2}\,dx\\
&=n!\int_{-\infty}^{\infty}e^{-x^2/2}\,dx
=\boxed{n!\sqrt{2\pi}}.
\end{aligned}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [19C](../../19c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

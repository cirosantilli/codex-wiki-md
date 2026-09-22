<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

An $L$-diffusion solves the [martingale problem](../../../../../../martingale-problem.md) for

$$
Lf(x)=b(x)f'(x)+\frac12\sigma(x)^2f''(x):
$$

for every $f\in C_c^2(\mathbb R)$,

$$
f(X_t)-f(X_0)-\int_0^tLf(X_s)\,ds
$$

is a local martingale. Applying this to cutoff approximations of $x$ and $x^2$ shows that

$$
M_t=X_t-X_0-\int_0^tb(X_s)\,ds
$$

is a continuous local martingale with

$$
[M]_t=\int_0^t\sigma(X_s)^2\,ds.
$$

Part b gives $M=\int|\sigma(X_s)|\,dW_s$. Changing the sign of $W$ predictably where $\sigma<0$, and filling the zero set with independent Brownian noise, produces a Brownian motion $B$ such that $M=\int\sigma(X_s)\,dB_s$. Thus

$$
\boxed{dX_t=b(X_t)\,dt+\sigma(X_t)\,dB_t.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

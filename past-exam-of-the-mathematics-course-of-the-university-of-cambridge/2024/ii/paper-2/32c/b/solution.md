<h1 id="32c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Since

$$
\frac{x}{x-1}=\frac1{1-x^{-1}}
\sim\sum_{j=0}^\infty x^{-j},
$$

we have

$$
\boxed{
f(x)\sim x^{-1}+\sum_{n=1}^\infty x^{-n+1}e^{-x}
=\sum_{n=0}^\infty\phi_n(x)}.
$$

Thus $a_n=1$ for every $n\geq0$.

Explicitly,

$$
\frac f{\phi_0}
=1+\frac{x^2e^{-x}}{x-1}\longrightarrow1.
$$

For $n\geq1$, the remainder after terms $0,\ldots,n-1$ is

$$
e^{-x}\left(\frac1{1-x^{-1}}
-\sum_{j=0}^{n-2}x^{-j}\right)
=\frac{x^{-n+1}e^{-x}}{1-x^{-1}}.
$$

Its ratio to $\phi_n$ tends to one, verifying every coefficient formula.

Because $e^{-x}=o(x^{-N})$ for every $N$, the exponentially small part is invisible to the power [sequence](../../../../../../sequence.md) $\psi_n=x^{-n}$. Hence

$$
\boxed{f(x)\sim x^{-1}}
$$

with coefficient one at $\psi_1$ and all other power coefficients zero.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [32C](../../32c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

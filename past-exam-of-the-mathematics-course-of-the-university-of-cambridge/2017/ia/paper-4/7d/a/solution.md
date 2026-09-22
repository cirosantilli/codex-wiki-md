<h1 id="7d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $n\ge2$, use the [binomial coefficient](../../../../../../binomial-coefficient.md) identity $(n/k)\binom{n-1}{k-1}=\binom nk$. It reduces the left side to $\binom{n-1}{k-1}(k/n)^{m-1}$. Put $t=(k-1)/(n-1)$. Then $k/n=((n-1)t+1)/n$, and the [binomial theorem](../../../../../../binomial-theorem.md) gives

$$
\left(\frac kn\right)^{m-1}=\sum_{\ell=0}^{m-1}\binom{m-1}{\ell}\frac{(n-1)^{m-1-\ell}}{n^{m-1}}t^{m-1-\ell}.
$$

Thus the required coefficients are

$$
\boxed{a_{n,m,\ell}=\binom{m-1}{\ell}\frac{(n-1)^{m-1-\ell}}{n^{m-1}},\qquad0\le\ell\le m-1.}
$$

For $m=1$ the sum has the single coefficient $a_{n,1,0}=1$. For $k=1$, the power $t^0$ denotes the constant [monomial](../../../../../../monomial.md) $1$.

The original PDF allows $n=1$, but its displayed ratio $(k-1)/(n-1)$ is then $0/0$. Literally that expression is undefined. The meaningful endpoint identity is obtained before normalization:

$$
\binom nk\left(\frac kn\right)^m=\binom{n-1}{k-1}\frac1{n^{m-1}}\sum_{\ell=0}^{m-1}\binom{m-1}{\ell}(k-1)^{m-1-\ell}.
$$

This [polynomial](../../../../../../polynomial-split.md) identity is valid at $n=k=1$, giving $1$ on both sides. The normalized formula and the [Bernstein monomial recurrence](../../../../../../bernstein-monomial-recurrence.md) below are used only for $n\ge2$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [7D](../../7d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

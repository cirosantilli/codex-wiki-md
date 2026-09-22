<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $m=k-1$, so the [Marsden identity](../../../../../../marsden-identity.md) is

$$
(x-t)^m=m!\sum_{i=1}^n\psi_i(x)N_i(t).
$$

Differentiating $m-j$ times with respect to $x$ gives

$$
\frac{(x-t)^j}{j!}
=\sum_{i=1}^n\psi_i^{(m-j)}(x)N_i(t),
\qquad 0\leq j\leq m.
$$

The exact [Taylor formula for a polynomial](../../../../../../taylor-formula-for-a-polynomial.md) is

$$
p(t)=\sum_{j=0}^m\frac{p^{(j)}(x)}{j!}(t-x)^j.
$$

Substitution of the differentiated Marsden identities yields

$$
\boxed{p(t)=\sum_{i=1}^n\lambda_i(p,x)N_i(t)},
$$

where

$$
\boxed{\lambda_i(p,x)=
\sum_{j=0}^{k-1}(-1)^j
\psi_i^{(k-1-j)}(x)p^{(j)}(x)}.
$$

Differentiating this expression for $\lambda_i$ produces two sums whose adjacent terms cancel. The uncancelled endpoints contain $\psi_i^{(k)}$ and $p^{(k)}$, both zero because the two functions have degree at most $k-1$. Thus

$$
\frac d{dx}\lambda_i(p,x)=0,
$$

so the [Marsden dual functional](../../../../../../marsden-dual-functional.md) $\lambda_i(p)$ is independent of the auxiliary point $x$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 318](../../../paper-318-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="6d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Since $xp_n-p_{n+1}$ has [degree of a polynomial](../../../../../../degree-of-a-polynomial.md) at most $n$, expand it in the [basis](../../../../../../basis.md) $p_0,\ldots,p_n$. Multiplication by $x$ is [self-adjoint](../../../../../../self-adjoint-operator.md) for this weighted [inner product](../../../../../../inner-product.md): $\langle xp,q\rangle=\langle p,xq\rangle$. For $k\leq n-2$, the polynomial $xp_k$ has degree at most $n-1$, so

$$
\langle xp_n-p_{n+1},p_k\rangle=\langle p_n,xp_k\rangle=0.
$$

Only the $p_n$ and $p_{n-1}$ coefficients remain. Taking their [inner products](../../../../../../inner-product.md) gives **the three-term recurrence**

$$
\boxed{p_{n+1}=(x-\alpha_n)p_n-\beta_n p_{n-1},\qquad \alpha_n=\frac{\langle xp_n,p_n\rangle}{\langle p_n,p_n\rangle},\quad \beta_n=\frac{\langle p_n,p_n\rangle}{\langle p_{n-1},p_{n-1}\rangle}>0\ (n\geq1).}
$$

For the second formula, $xp_{n-1}=p_n+$ a polynomial of lower degree, hence $\langle xp_n,p_{n-1}\rangle=\langle p_n,xp_{n-1}\rangle=\langle p_n,p_n\rangle$. At $n=0$, take $p_{-1}=0$, $\beta_0=0$ and the same formula for $\alpha_0$. Positivity of the weight ensures that all the squared [norms](../../../../../../norm.md) in the denominators are nonzero.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6D](../../6d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

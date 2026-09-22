<h1 id="17c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Insert the exact data $y(t)=P(t)$ into the [linear multistep method](../../../../../../linear-multistep-method.md). Its local residual is the linear functional

$$
\mathcal L_h[P]
=\sum_{k=0}^s\rho_kP(t_{n+k})
-h\sum_{k=0}^s\sigma_kP'(t_{n+k}).
$$

Taylor expansion about $t_n$ shows that a method has order $p$ exactly when this functional annihilates the monomials $1,t,\ldots,t^p$; by linearity this is equivalent to annihilating every polynomial of degree at most $p$. This is precisely

$$
\boxed{
\sum_{k=0}^s\rho_kP(t_{n+k})
=h\sum_{k=0}^s\sigma_kP'(t_{n+k})}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [17C](../../17c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

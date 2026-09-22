<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The remainders in the [sieve distribution](../../../../../../sieve-distribution.md) are defined by

$$
r(d)=A_d-Xg(d),\qquad A_d=\sum_{d\mid n}a_n.
$$

Multiply the pointwise inequality from part (a) by $a_n\geq0$ and sum. Finite rearrangement gives

$$
S\leq\sum_d\lambda_dA_d
=X\sum_d\lambda_dg(d)+\sum_{d\leq D}\lambda_dr(d).
$$

To identify the main quadratic form, put $h(t)=\prod_{p\mid t}(g(p)^{-1}-1)$. For [squarefree integers](../../../../../../squarefree-integer.md) $u,v$, [multiplicativity](../../../../../../multiplicativity-of-an-arithmetic-function.md) gives

$$
\sum_{t\mid(u,v)}h(t)=\prod_{p\mid(u,v)}g(p)^{-1},\qquad
g([u,v])=g(u)g(v)\sum_{t\mid(u,v)}h(t).
$$

The second identity is also valid if $u$ or $v$ is not [squarefree](../../../../../../squarefree-integer.md): both sides then vanish. Therefore the [Selberg sieve diagonalization](../../../../../../selberg-sieve-diagonalization.md) gives

$$
\sum_d\lambda_dg(d)
=\sum_{u,v\leq L}\rho_u\rho_vg([u,v])
=\sum_{t\leq L}h(t)\left(\sum_{\substack{m\leq L\\t\mid m}}g(m)\rho_m\right)^2
=\Sigma.
$$

This proves $S\leq X\Sigma+\sum_{d\leq D}\lambda_dr(d)$. Notice that the hypotheses do not force $\rho_m$ to vanish on non-[squarefree integers](../../../../../../squarefree-integer.md); those coefficients simply make no contribution to this main quadratic form because $g(m)=0$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

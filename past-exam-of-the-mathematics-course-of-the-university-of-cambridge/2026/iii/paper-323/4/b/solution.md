<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $\rho=p\rho_1+(1-p)\rho_2$. The [operator inequality](../../../../../../lowner-order.md) $\rho\geq p\rho_1$ and the [operator monotonicity of logarithm](../../../../../../operator-monotonicity-of-logarithm.md) give, on the support of $\rho_1$,

$$
\log\rho\geq\log(p\rho_1)
=(\log p)I+\log\rho_1.
$$

Consequently,

$$
-p\operatorname{Tr}(\rho_1\log\rho)
\leq pS(\rho_1)-p\log p.
$$

The corresponding inequality from $\rho\geq(1-p)\rho_2$ yields

$$
-(1-p)\operatorname{Tr}(\rho_2\log\rho)
\leq(1-p)S(\rho_2)-(1-p)\log(1-p).
$$

Adding these inequalities and using $S(\rho)=-\operatorname{Tr}(\rho\log\rho)$ proves the [entropy bound for a binary mixture](../../../../../../entropy-bound-for-a-binary-mixture.md):

$$
\boxed{S(\rho)\leq pS(\rho_1)+(1-p)S(\rho_2)+H(p)}.
$$

Singular states follow by adding a positive multiple of the identity and taking a [limit](../../../../../../limit-of-a-function.md); the endpoint cases use $0\log0=0$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For the recovered $a,z$ of the preceding part, compute the forward ratio $R$ from part (i). The reverse [probability density function](../../../../../../../probability-density-function.md) ratio and reverse [Jacobian determinant](../../../../../../../jacobian-determinant.md) invert every factor, so

$$
\boxed{\alpha_\downarrow=\min(1,R^{-1}).}
$$

Equivalently, with $L_k(a;v)$ denoting the Gaussian regression [likelihood](../../../../../../../likelihood-function.md),

$$
\alpha_\downarrow=\min\left\{1,\frac{\rho_kb_k}{\rho_{k+1}d_{k+1}}\frac{L_k(a;v)p_k(a)q(z)}{L_{k+1}(a';v)p_{k+1}(a')}\right\}.
$$

The factor $q(z)$ is present even though no random variable is generated during the death proposal: it is the [probability density function](../../../../../../../probability-density-function.md) of the auxiliary variable required by the reverse birth. These reciprocal rules give [detailed balance](../../../../../../../detailed-balance.md) on the paired dimension-matching moves.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 40](../../../../paper-40-split.md)
5. [Iii](../../../../split.md)
6. [2002](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

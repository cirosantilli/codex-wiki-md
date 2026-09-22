<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a sequence trapped between the fixed barriers, let $M$ bound their absolute values and put $A=\sup_{|s|\leq M}|V'(s)|$. The [mean value theorem](../../../../../../mean-value-theorem.md) gives

$$
\|V(u_{k-1})\|_{C^{0,\alpha}}\leq C_0+A\|u_{k-1}\|_{C^{0,\alpha}}.
$$

The [global Schauder estimate](../../../../../../global-schauder-estimate.md), including the fixed boundary data $\psi$, and $\|u_k\|_\infty\leq M$ imply

$$
\|u_k\|_{C^{2,\alpha}}\leq KA\|u_{k-1}\|_{C^{0,\alpha}}+C_1.
$$

Apply the supplied [Hölder interpolation inequality](../../../../../../holder-interpolation-inequality.md) with $KA\varepsilon\leq1/2$. Its remaining supremum-norm term is bounded by $M$, yielding

$$
\boxed{\|u_k\|_{C^{2,\alpha}}\leq\tfrac12\|u_{k-1}\|_{C^{2,\alpha}}+C.}
$$

If $A=0$, the stronger bound without a previous-iterate term holds directly. The constant depends on the fixed domain, exponent, barriers, boundary data and $V$, independently of $k$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

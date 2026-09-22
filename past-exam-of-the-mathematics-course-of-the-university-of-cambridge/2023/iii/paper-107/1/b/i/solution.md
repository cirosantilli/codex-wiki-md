<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Choose a [cutoff function](../../../../../../../cutoff-function.md) $\eta$ supported in $B_\rho(x)$, equal to one on $B_{\rho'}(x)$, and satisfying $|D\eta|\leq(\rho-\rho')^{-1}$. Use $\eta^2u$ as a [test function](../../../../../../../test-function.md) in the [weak formulation](../../../../../../../weak-formulation.md):

$$
0=\int D u\mathbin\cdot D(\eta^2u)
=\int\eta^2|Du|^2+2\int\eta u,Du\mathbin\cdot D\eta.
$$

The [Cauchy-Schwarz inequality](../../../../../../../cauchy-schwarz-inequality.md) followed by [Young inequality](../../../../../../../young-s-inequality-for-products.md) gives

$$
\int\eta^2|Du|^2\leq4\int u^2|D\eta|^2,
$$

and hence

$$
\int_{B_{\rho'}(x)}|Du|^2
\leq\frac{4}{(\rho-\rho')^2}\int_{B_\rho(x)}|u|^2.
$$

This is the [Caccioppoli inequality](../../../../../../../caccioppoli-inequality.md). The numerical constant is convention-dependent and is normally absorbed into the displayed estimate; replacing the radii by fixed intermediate radii gives the stated form with one universal constant.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 107](../../../../paper-107-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

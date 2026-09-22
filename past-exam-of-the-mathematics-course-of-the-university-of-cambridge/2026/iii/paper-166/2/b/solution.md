<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose a [number field](../../../../../../number-field.md) $L$ containing $\alpha_1,\ldots,\alpha_k$. At every place $v$ of $L$, put

$$
A_v=\prod_{j=1}^k\max(1,|\alpha_j|_v)^{n_j}.
$$

The [triangle inequality](../../../../../../triangle-inequality.md) gives

$$
\max\{|P(\boldsymbol\alpha)|_v,|Q(\boldsymbol\alpha)|_v\}
\leq c_vA_v,
$$

where $c_v=1$ at every non-Archimedean place because the coefficients are [integers](../../../../../../integer.md), while at an Archimedean place one may take

$$
c_v=\max\{\mathcal L(P),\mathcal L(Q)\}.
$$

Raise these inequalities to the local weights and multiply over all places. The definition of the [Absolute multiplicative Weil height](../../../../../../absolute-multiplicative-weil-height.md) and the [product formula](../../../../../../product-formula.md) then give

$$
H\left(\frac{P(\alpha_1,\ldots,\alpha_k)}
{Q(\alpha_1,\ldots,\alpha_k)}\right)
\leq
\max\{\mathcal L(P),\mathcal L(Q)\}
\prod_{j=1}^kH(\alpha_j)^{n_j}.
$$

This is the [height bound for a polynomial evaluation](../../../../../../height-bound-for-a-polynomial-evaluation.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 166](../../../paper-166-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

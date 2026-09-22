<h1 id="1a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use [suffix notation](../../../../../../einstein-notation.md), summing repeated indices, and the [Levi-Civita symbol](../../../../../../levi-civita-symbol.md) convention $(A\times B)_i=\epsilon_{ijk}A_jB_k$. Contracting the outer symbol with the symbol from the second [cross product](../../../../../../cross-product.md) gives the [epsilon-delta identity](../../../../../../contraction-of-two-levi-civita-symbols.md)

$$
\epsilon_{ijk}\epsilon_{kpq}=\delta_{ip}\delta_{jq}-\delta_{iq}\delta_{jp},
$$

where $\delta$ is the [Kronecker delta](../../../../../../kronecker-delta.md). Thus

$$
\begin{aligned}
\bigl((A\times B)\times(A\times C)\bigr)_i
&=\epsilon_{ijk}\epsilon_{j\ell m}\epsilon_{kpq}A_\ell B_mA_pC_q\\
&=(\delta_{ip}\delta_{jq}-\delta_{iq}\delta_{jp})\epsilon_{j\ell m}A_\ell B_mA_pC_q\\
&=A_i\epsilon_{q\ell m}C_qA_\ell B_m
-C_i\epsilon_{p\ell m}A_pA_\ell B_m\\
&=A_i\epsilon_{\ell mq}A_\ell B_mC_q.
\end{aligned}
$$

The second term is zero because $A_pA_\ell$ is symmetric in $p,\ell$ and the [Levi-Civita symbol](../../../../../../levi-civita-symbol.md) is antisymmetric. The cyclic rearrangement of the remaining symbol has positive sign. Its contraction is the [scalar triple product](../../../../../../scalar-triple-product.md) $A\cdot(B\times C)$. Hence

$$
\boxed{(A\times B)\times(A\times C)=(A\cdot(B\times C))A.}
$$

This [cross products with a common vector](../../../../../../cross-products-with-a-common-vector.md) identity requires no independence assumption, so it also covers zero or parallel vectors.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1A](../../1a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First separate the [symmetric tensor](../../../../../symmetric-tensor.md) and [antisymmetric tensor](../../../../../antisymmetric-tensor.md) parts:

$$
P_{ij}=\tfrac12(P_{ij}+P_{ji})+\tfrac12(P_{ij}-P_{ji}).
$$

The [trace](../../../../../matrix-trace.md) of the antisymmetric part vanishes. In three dimensions, remove one third of the trace from the symmetric part, and identify the remaining antisymmetric part with an [axial vector](../../../../../pseudovector.md). The [scalar, symmetric-traceless and axial tensor decomposition](../../../../../scalar-symmetric-traceless-and-axial-tensor-decomposition.md) is

$$
\boxed{P=\tfrac13P_{ii},\qquad S_{ij}=\tfrac12(P_{ij}+P_{ji})-\tfrac13P_{kk}\delta_{ij},\qquad A_k=\tfrac12\epsilon_{kij}P_{ij}.}
$$

Here $S_{ji}=S_{ij}$ and $S_{ii}=P_{ii}-P_{kk}=0$. The [contraction of two Levi-Civita symbols](../../../../../contraction-of-two-levi-civita-symbols.md) verifies the reconstruction:

$$
\epsilon_{ijk}A_k=\tfrac12\epsilon_{ijk}\epsilon_{k\ell m}P_{\ell m}=\tfrac12(\delta_{i\ell}\delta_{jm}-\delta_{im}\delta_{j\ell})P_{\ell m}=\tfrac12(P_{ij}-P_{ji}).
$$

Therefore

$$
\boxed{P_{ij}=P\delta_{ij}+S_{ij}+\epsilon_{ijk}A_k.}
$$

The pieces contain $1$, $5$ and $3$ independent components respectively, accounting for all nine entries. Taking the trace, then the traceless symmetric part, then the antisymmetric part shows that the decomposition is unique.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

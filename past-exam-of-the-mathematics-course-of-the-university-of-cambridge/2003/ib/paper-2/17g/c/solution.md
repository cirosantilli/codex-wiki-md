<h1 id="17g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Taking [traces](../../../../../../matrix-trace.md) in the defining equation gives $\operatorname{tr}C+\overline{\operatorname{tr}C}=2\operatorname{tr}C$, so the [trace](../../../../../../matrix-trace.md) is real. Put $a=\operatorname{tr}C/2$. Then $K=C-aI$ is traceless and satisfies $K^*=-K$, so $-iK$ is a traceless [Hermitian matrix](../../../../../../hermitian-operator.md). Hence every element has a unique representation

$$
C=aI+i\sum_jv_jA_j,\qquad a,v_j\in\mathbb R.
$$

Conversely each such [matrix](../../../../../../matrix.md) satisfies the defining equation. This proves **$Q$ is a real four-dimensional vector space**, with [basis](../../../../../../basis.md) $I,iA_1,iA_2,iA_3$.

Substitution into the given map gives

$$
\boxed{\Phi\left(aI+i\sum_jv_jA_j\right)=aI-\sum_jv_jA_j.}
$$

Its values are Hermitian, and it acts on real coordinates by $(a,v_1,v_2,v_3)\mapsto(a,-v_1,-v_2,-v_3)$. This invertible real linear coordinate transformation proves the required isomorphism. The inverse sends $aI+\sum_ju_jA_j$ to $aI-i\sum_ju_jA_j$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [17G](../../17g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="a/1/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Give $V$ a $k[t]$-[module](../../../../../../module-mathematics.md) structure by $t\cdot v=\alpha v$. A finite [vector space basis](../../../../../../basis.md) generates it as a [module](../../../../../../module-mathematics.md). It is a [torsion module](../../../../../../torsion-module.md): the [Cayley-Hamilton theorem](../../../../../../cayley-hamilton-theorem-split.md) gives a nonzero polynomial annihilating all of $V$. Since $k[t]$ is a [Euclidean domain](../../../../../../euclidean-domain.md), cyclic decomposition gives

$$
V\cong\bigoplus_{j=1}^s k[t]/(f_j),\qquad f_1\mid\cdots\mid f_s,
$$

with monic nonconstant [invariant factors of a linear operator](../../../../../../invariant-factors-of-a-linear-operator.md) $f_j$ and no free summand. On $k[t]/(f_j)$, use the [basis](../../../../../../basis.md) $1,t,\ldots,t^{\deg f_j-1}$. Multiplication by $t$ then has the [companion matrix](../../../../../../companion-matrix.md) $C(f_j)$, because the relation $f_j(t)=0$ expresses the last power in terms of earlier ones. Concatenating these [bases](../../../../../../basis.md) yields

$$
\boxed{\operatorname{diag}(C(f_1),\ldots,C(f_s)),}
$$

the [rational canonical form](../../../../../../rational-canonical-form.md) of $\alpha$. In particular, its [minimal polynomial](../../../../../../minimal-polynomial.md) is $f_s$ and its [characteristic polynomial](../../../../../../characteristic-polynomial.md) is $\prod_jf_j$.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [A](../../../../a.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the algebra course of the University of Oxford](../../../../../split.md)
7. [Algebra course of the University of Oxford](../../../../../../algebra-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)

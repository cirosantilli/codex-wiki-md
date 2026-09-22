<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

First suppose $\operatorname{char}k\ne2$. The quadratic form has rank $n>2$, so it is irreducible: a reducible homogeneous quadratic would be a product of two linear forms, whose associated symmetric matrix has rank at most two. Thus

$$
A=k[t_1,\ldots,t_n]/(t_1^2+\cdots+t_n^2)
$$

is a domain of dimension $n-1$. Its gradient is $(2t_1,\ldots,2t_n)$, so the [Jacobian criterion](../../../../../../jacobian-criterion.md) shows that the only singular point is the origin. Its codimension is $n-1\ge2$, giving regularity at all codimension-one points, the $(R_1)$ condition.

At every localization the polynomial ambient ring is regular and hence a [Cohen-Macaulay ring](../../../../../../cohen-macaulay-ring.md). The nonzero quadratic equation is a nonzero divisor; quotienting by it decreases both depth and dimension by one. Hence the hypersurface [local rings](../../../../../../local-ring.md) remain Cohen-Macaulay, so their depth is their dimension and in particular at least $\min(2,\dim)$. This verifies $(S_2)$. The [Serre criterion for normality](../../../../../../serre-s-criterion-for-normality.md) now yields **$\boxed{X\text{ is normal}}$**, establishing [normality of a quadratic cone](../../../../../../normality-of-a-quadratic-cone.md) with all its hypotheses checked.

In characteristic two, $t_1^2+\cdots+t_n^2=(t_1+\cdots+t_n)^2$. The reduced zero variety is therefore the hyperplane $t_1+\cdots+t_n=0$, isomorphic to affine $(n-1)$-space, and its polynomial [coordinate ring](../../../../../../coordinate-ring.md) is integrally closed. Thus the reduced variety is normal in this case too. If one instead keeps the nonreduced hypersurface scheme defined by the squared equation, its [coordinate ring](../../../../../../coordinate-ring.md) has a nonzero square-zero class and is not normal. The variety interpretation in the question requires the reduced zero set.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

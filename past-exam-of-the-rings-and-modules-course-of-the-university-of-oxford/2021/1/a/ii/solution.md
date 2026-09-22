<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Regard $\mathbb R[X,Y]$ as the [polynomial ring](../../../../../polynomial-ring.md) $(\mathbb R[X])[Y]$. The [coefficient](../../../../../coefficient.md) [ring](../../../../../ring.md) $\mathbb R[X]$ is a [Euclidean domain](../../../../../euclidean-domain.md), hence a [principal ideal domain](../../../../../principal-ideal-domain.md). The element $X$ is a [prime element](../../../../../prime-element.md): the [quotient ring](../../../../../quotient-ring.md) $\mathbb R[X]/(X)\cong\mathbb R$ is an [integral domain](../../../../../integral-domain.md).

The [monic polynomial](../../../../../monic-polynomial.md) $Y^2+X$ has its other [coefficients](../../../../../coefficient.md) divisible by $X$, while $X^2\nmid X$. Part (a)(i), with $X$ playing the role of $p$ and $Y$ the [indeterminate](../../../../../indeterminate.md), proves that $Y^2+X$ is an [irreducible polynomial](../../../../../irreducible-polynomial.md).

Now use the [automorphism of a polynomial ring](../../../../../automorphism-of-a-polynomial-ring.md)

$$
\tau:\mathbb R[X,Y]\longrightarrow\mathbb R[X,Y],\qquad
\tau(X)=X,\quad\tau(Y)=Y+1.
$$

Its inverse fixes $X$ and sends $Y$ to $Y-1$. A [ring isomorphism](../../../../../ring-isomorphism.md) preserves [units](../../../../../unit-in-a-ring.md) and factorizations, hence preserves [irreducible elements](../../../../../irreducible-element.md). Since

$$
\tau(Y^2+X)=(Y+1)^2+X=Y^2+2Y+1+X,
$$

we obtain

$$
\boxed{Y^2+X\text{ and }Y^2+2Y+1+X\text{ are irreducible in }\mathbb R[X,Y]}.
$$

Applying the [Eisenstein criterion](../../../../../eisenstein-criterion.md) directly to the second expression with the [prime element](../../../../../prime-element.md) $X$ would fail, since $X\nmid2$; the change of [indeterminate](../../../../../indeterminate.md) supplies the required argument.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the rings and modules course of the University of Oxford](../../../../split.md)
6. [Rings and modules course of the University of Oxford](../../../../../rings-and-modules-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

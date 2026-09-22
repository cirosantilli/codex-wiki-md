<h1 id="21f/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write the target coordinates as $x_1,x_2,x_3,x_4$. Every image point satisfies $x_3=x_2^2$ and $x_4=x_1x_2$. Conversely any point satisfying these equations is obtained by taking $t=x_2$, $u=x_1$. Hence the image is the closed [affine variety](../../../../../../affine-algebraic-set.md)

$$
\boxed{X=V(x_3-x_2^2,\ x_4-x_1x_2)}.
$$

The substitution homomorphism $k[x_1,x_2,x_3,x_4]\to k[u,t]$ has kernel exactly the ideal $J=(x_3-x_2^2,x_4-x_1x_2)$: reduce any [polynomial](../../../../../../polynomial-split.md) by these two relations to a [polynomial](../../../../../../polynomial-split.md) in $x_1,x_2$, which vanishes after substitution only if it is zero. Equivalently the quotient by $J$ is $k[x_1,x_2]$, so $J$ is prime. Since $k$ is algebraically closed, or directly by the same polynomial-vanishing argument, **$I(X)=J$**.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [21F](../../21f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Here the inverse in the [elliptic curve group law](../../../../../../elliptic-curve-group-law-from-riemann-roch.md) is $(x,y)\mapsto(x,-y-1)$. For $P_0+P_1$, the line is $y=2-2x$. Substitution in the [Weierstrass equation of an elliptic curve](../../../../../../weierstrass-equation-of-an-elliptic-curve.md) gives

$$
x^3-7x+6-\bigl((2-2x)^2+(2-2x)\bigr)=x(x-1)(x-3).
$$

The third intersection is $(3,-4)$, so reflection gives

$$
\boxed{P_0+P_1=(3,3).}
$$

For the difference, first take $-P_1=(1,-1)$. The line through $P_0$ and $-P_1$ is $y=2-3x$, and now the intersection polynomial is $x(x-1)(x-8)$. Its third point is $(8,-22)$, giving

$$
\boxed{P_0-P_1=(8,21).}
$$

Finally, implicit [differentiation](../../../../../../differentiation.md) gives $(2y+1)y'=3x^2-7$. The [tangent line](../../../../../../tangent-line.md) at $P_1$ therefore has slope $-4$ and equation $y=4-4x$. Its intersection polynomial factors as $(x-1)^2(x-14)$. The double root records the [intersection multiplicity](../../../../../../intersection-multiplicity.md) of the tangent, and the remaining intersection is $(14,-52)$. Hence

$$
\boxed{2P_1=(14,51).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

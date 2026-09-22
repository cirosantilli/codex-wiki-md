<h1 id="9/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Squaring with the product law gives

$$
A(a,b,c)^2=A(2a,\ 2b+ac,\ 2c).
$$

Equality to the [identity matrix](../../../../../identity-matrix.md) requires $2a=2c=0$ in $\mathbb F_5$. Since 2 has a multiplicative inverse modulo 5, this forces $a=c=0$. The middle condition then gives $2b=0$, hence $b=0$. Therefore

$$
\boxed{\{A\in G:A^2=I\}=\{I\}.}
$$

This agrees with [Lagrange's theorem](../../../../../lagrange-s-theorem.md): a group of odd order has no element of order two.

The subset specified by $b\ne0$ **is not a subgroup**. It omits the [identity element](../../../../../identity-element.md). It also fails [closure](../../../../../closure-topology.md): both $A(0,1,0)$ and $A(0,4,0)$ lie in it, but their product is $A(0,0,0)=I$, whose $b$ coordinate is zero.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [9](../../9.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

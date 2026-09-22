<h1 id="a/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A finite [straightedge and compass construction](../../../../straightedge-and-compass-construction-split.md) repeatedly draws the line through two available distinct points or the [circle](../../../../circle.md) with an available center and an available distance as radius, and adjoins isolated intersections of two such lines or [circles](../../../../circle.md). A finite set is constructible when its points occur after finitely many such steps, starting with the specified points.

If the current coordinate [field](../../../../field.md) is $F$, intersections of two lines solve [linear equations](../../../../linear-equation.md) over $F$. A line and a [circle](../../../../circle.md) lead to a [quadratic equation](../../../../quadratic-equation.md) over $F$. For two distinct [circles](../../../../circle.md), subtraction of their equations gives a line, reducing to the previous case. Thus each step adjoins coordinates in an extension of degree one or two. The [tower law](../../../../tower-law.md) gives a finite tower of quadratic-or-trivial [field extensions](../../../../field-extension.md) containing all output coordinates. If the final coordinate [field](../../../../field.md) contains $K_0$, then

$$
\boxed{[K:K_0]=2^r\quad\text{for some integer }r\ge0,}
$$

because its degree divides the power-of-two degree of that tower.

Two implicit qualifications are necessary for this degree statement. The output is obtained in finitely many steps; the aggregate of infinitely many individually constructible points need not generate a finite extension. Also, unless the output retains the original coordinates, $K$ need not contain $K_0$. In that case the degree statement applies to the compositum $K_0K$, rather than an undefined $[K:K_0]$. The heptagon application explicitly includes $S_0$, so neither issue obstructs it.

Here $K_0=\mathbb Q$, and a vertex adjacent to $(1,0)$ has first coordinate $c=\cos(2\pi/7)$, so $\mathbb Q(c)\subseteq K$. Let $\zeta=e^{2\pi i/7}$. The [cyclotomic polynomial](../../../../cyclotomic-polynomial.md) $1+X+\cdots+X^6$ is [irreducible](../../../../irreducible-representation.md), giving $[\mathbb Q(\zeta):\mathbb Q]=6$. Since $\zeta+\zeta^{-1}=2c$, it satisfies $X^2-2cX+1$ over $\mathbb Q(c)$. The element $\zeta$ is nonreal while $\mathbb Q(c)\subset\mathbb R$, so this relative degree is exactly two. By the [tower law](../../../../tower-law.md),

$$
[\mathbb Q(c):\mathbb Q]=3.
$$

If the regular [regular heptagon](../../../../regular-heptagon.md) were constructible, this degree would divide $[K:\mathbb Q]=2^r$, impossible. Therefore **the [regular heptagon](../../../../regular-heptagon.md) is not constructible** from the given unit segment.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the number theory course of the University of Oxford](../../../split.md)
5. [Number theory course of the University of Oxford](../../../../number-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use [cohomology](../../../../../cohomology-split.md) with coefficients in $\mathbb F_2=\mathbb Z_2$. The [cellular homology of real projective space](../../../../../cellular-homology-of-real-projective-space.md) has one cell in degrees zero, one and two, and its boundary coefficients become zero modulo two. Hence there is a one-dimensional cohomology group in each of those degrees. Let $x\in H^1(P;\mathbb F_2)$ be the [Poincare dual](../../../../../poincare-dual.md) of a projective line. Two distinct projective lines intersect transversely in one point, so $\langle x^2,[P]_2\rangle=1$. Thus

$$
\boxed{H^*(P;\mathbb F_2)=\mathbb F_2[x]/(x^3),\qquad |x|=1.}
$$

This is the [mod-two cohomology ring of real projective space](../../../../../mod-two-cohomology-ring-of-real-projective-space.md) in dimension two. The [Künneth theorem](../../../../../kunneth-theorem.md) over a field makes the cross product an isomorphism of graded rings. Writing $x,y$ for the factor pullbacks gives

$$
\boxed{H^*(P\times P;\mathbb F_2)=\mathbb F_2[x,y]/(x^3,y^3).}
$$

There are no additional signs over $\mathbb F_2$.

The obstruction to a graph avoiding the diagonal is the [mod-two diagonal class of the real projective plane](../../../../../mod-two-diagonal-class-of-the-real-projective-plane.md). Its dual class $D\in H^2(P\times P;\mathbb F_2)$ is determined by

$$
\langle D\smile z,[P\times P]_2\rangle=\langle i^*z,[P]_2\rangle,
$$

where $i:P\to P\times P$ is the [diagonal embedding](../../../../../diagonal-map.md). Test $z=x^2,xy,y^2$. Each diagonal pullback is $x^2$, with evaluation one. Since $x^2y^2$ is the product's top generator, comparison of coefficients gives

$$
D=x^2+xy+y^2.
$$

If the submanifold were the graph of a smooth map $f:P\to P$, its parametrization would be $j=(\mathrm{id},f)$. For some $\varepsilon\in\mathbb F_2$, $f^*x=\varepsilon x$, and therefore

$$
j^*D=(1+\varepsilon+\varepsilon^2)x^2=x^2\ne0.
$$

On the other hand, the [Poincare dual](../../../../../poincare-dual.md) of the diagonal comes from its relative [Thom class](../../../../../thom-class.md) in $H^2(P\times P,(P\times P)\setminus\Delta;\mathbb F_2)$. It restricts to zero on the complement. A graph disjoint from the diagonal would factor through that complement and force $j^*D=0$, a contradiction. **Such a submanifold cannot be the graph of a smooth map $P\to P$.** The relative Thom-class argument also applies to continuous self-maps.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 16](../../paper-16-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

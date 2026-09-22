<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For each $h\in g^G\cap H$, count the solutions of $x^{-1}gx=h$. Once a solution $x_0$ is fixed, every solution is uniquely $cx_0$ with $c\in C_G(g)$, the [centralizer](../../../../centralizer.md) of $g$. Thus each $h$ contributes $|C_G(g)|\chi_W(h)$ to the sum in part (a).

The [orbit-stabilizer theorem](../../../../orbit-stabilizer-theorem.md) for the [conjugation action](../../../../conjugation-action.md) gives $|C_G(g)|=|G|/|g^G|$. The intersection $g^G\cap H$ is the disjoint union of the [conjugacy classes](../../../../conjugacy-class.md) $h_1^H,\ldots,h_\ell^H$, and the [character](../../../../character-of-a-representation.md) $\chi_W$ is constant on each such [conjugacy class](../../../../conjugacy-class.md). Hence

$$
\chi_V(g)=\frac{|C_G(g)|}{|H|}\sum_{h\in g^G\cap H}\chi_W(h)
=\boxed{\frac{|G|}{|H|}\sum_{i=1}^{\ell}\frac{|h_i^H|}{|g^G|}\chi_W(h_i)}.
$$

If the intersection is empty, the empty sum gives zero. This is the [conjugacy-class formula for an induced character](../../../../conjugacy-class-formula-for-an-induced-character.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the introduction to representation theory course of the University of Oxford](../../../split.md)
5. [Introduction to representation theory course of the University of Oxford](../../../../introduction-to-representation-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

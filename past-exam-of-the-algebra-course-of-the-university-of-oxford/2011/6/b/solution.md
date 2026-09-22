<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Over $\mathbb F_q$, the first nonzero column of an invertible $2\times2$ [matrix](../../../../matrix.md) has $q^2-1$ choices and the second has $q^2-q$ choices. The surjective [determinant](../../../../determinant.md) homomorphism onto $\mathbb F_q^\times$ has [kernel](../../../../kernel-of-a-linear-map-split.md) $\operatorname{SL}_2(q)$. Thus

$$
\boxed{|\operatorname{SL}_2(8)|=\frac{(8^2-1)(8^2-8)}{8-1}=504.}
$$

It acts on the nine one-dimensional subspaces of $\mathbb F_8^2$, namely the [projective line](../../../../projective-line.md) $\mathbb F_8\cup\{\infty\}$, by fractional linear transformations. Any element acting trivially fixes $0,\infty,1$, which forces it to be scalar. A scalar [matrix](../../../../matrix.md) in $\operatorname{SL}_2(8)$ has $a^2=1$; in characteristic two this implies $a=1$. Thus the action is faithful.

The action is transitive: any nonzero vector can be completed to a [determinant](../../../../determinant.md)-one [basis](../../../../basis.md), so any line can be reached. The [stabilizer](../../../../stabilizer-subgroup.md) of $\infty=[1:0]$ is

$$
\boxed{\left\{\begin{pmatrix}a&b\\0&a^{-1}\end{pmatrix}:
 a\in\mathbb F_8^\times,\ b\in\mathbb F_8\right\}
\cong (C_2)^3\rtimes C_7.}
$$

On finite points this is $x\mapsto a^2x+ab$. Squaring permutes the seven nonzero field elements, so these are exactly the affine maps $x\mapsto ux+v$. In particular translations act transitively on all eight finite points. Thus the full action is doubly transitive. The point [stabilizer](../../../../stabilizer-subgroup.md) has order $8\cdot7=56$, and all point [stabilizers](../../../../stabilizer-subgroup.md) are conjugate.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the algebra course of the University of Oxford](../../../split.md)
5. [Algebra course of the University of Oxford](../../../../algebra-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

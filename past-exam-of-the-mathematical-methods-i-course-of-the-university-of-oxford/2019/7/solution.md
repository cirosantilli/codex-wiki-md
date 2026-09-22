<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

Write the given [matrix](../../../matrix.md) as $A$. Expanding its [characteristic polynomial](../../../characteristic-polynomial.md) along the middle column gives

$$
\begin{aligned}
\det(\lambda I-A)
&=(\lambda+2)\big[(\lambda-7)(\lambda+8)+54\big]\\
&=(\lambda+2)(\lambda^2+\lambda-2)
=(\lambda-1)(\lambda+2)^2.
\end{aligned}
$$

Thus the [eigenvalues](../../../eigenvalue.md) are $1,-2,-2$, counted with [algebraic multiplicity](../../../algebraic-multiplicity.md).

For $\lambda=1$, solving $(A-I)v=0$ gives $z=2x$ and $y=-x$. For $\lambda=-2$, solving $(A+2I)v=0$ gives $z=3x$, with $y$ free. A convenient [eigenbasis](../../../eigenbasis.md) is therefore

$$
\boxed{\begin{array}{c|c}
\lambda&\text{eigenvector}\\\hline
1&(1,-1,2)^T\\
-2&(1,0,3)^T\\
-2&(0,1,0)^T
\end{array}}
$$

The last two [eigenvectors](../../../eigenvector.md) span the two-dimensional [eigenspace](../../../eigenspace.md) for $-2$. The three columns have [determinant](../../../determinant.md) $-1$, so they are linearly independent and form a [basis](../../../basis.md) of $\mathbb R^3$. In particular the repeated [eigenvalue](../../../eigenvalue.md) causes no failure of [diagonalizability](../../../diagonalizable-matrix.md) here.

## ↑ Ancestors (11)

1. [7](../7.md)
2. [2019](../../2019-split.md)
3. [Past exam of the mathematical methods I course of the University of Oxford](../../split.md)
4. [Mathematical methods I course of the University of Oxford](../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)

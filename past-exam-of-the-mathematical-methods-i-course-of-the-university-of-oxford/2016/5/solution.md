<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The equations are an [eigenvalue problem](../../../eigenvalue-problem.md) for the [matrix](../../../matrix.md)

$$
A=\begin{pmatrix}2&-2&1\\2&-3&2\\-1&2&0\end{pmatrix}.
$$

A nonzero solution requires $\det(\lambda I-A)=0$. Expanding gives

$$
\det(\lambda I-A)=(\lambda-1)^2(\lambda+3),\qquad \boxed{\lambda=1\ \text{or}\ -3.}
$$

[Row reduction](../../../gaussian-elimination.md) gives the complete [eigenspaces](../../../eigenspace.md):

$$
\boxed{\begin{aligned}
\lambda=1:&\quad (x,y,z)=s(2,1,0)+t(-1,0,1),\qquad s,t\in\mathbb R,\\
\lambda=-3:&\quad (x,y,z)=u(-1,-2,1),\qquad u\in\mathbb R.
\end{aligned}}
$$

For $\lambda=1$ the solutions form the [plane](../../../plane.md) $x-2y+z=0$ through the origin; for $\lambda=-3$ they form a [line](../../../straight-line.md) through the origin. Exclude the zero vector when requiring a nontrivial solution. The repeated [eigenvalue](../../../eigenvalue.md) $1$ has a two-dimensional [eigenspace](../../../eigenspace.md); there are three independent [eigenvectors](../../../eigenvector.md) in total. This matrix is not symmetric, so its different [eigenspaces](../../../eigenspace.md) need not be mutually [orthogonal](../../../orthogonal-vectors.md).

## ↑ Ancestors (11)

1. [5](../5.md)
2. [2016](../../2016-split.md)
3. [Past exam of the mathematical methods I course of the University of Oxford](../../split.md)
4. [Mathematical methods I course of the University of Oxford](../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)

<h1 id="9/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write the displacement as $\mathbf x=\mathbf a\cos(\omega t+\phi)$. The [generalized eigenvalue problem](../../../../generalized-eigenvalue-problem.md) is

$$
k\begin{pmatrix}1&-1&0\\-1&2&-1\\0&-1&1\end{pmatrix}\mathbf a=\omega^2\operatorname{diag}(m,M,m)\mathbf a.
$$

The symmetry of the two end atoms suggests an end-antisymmetric shape $(1,0,-1)$ and two end-symmetric shapes. Direct substitution gives the [normal modes of three masses connected by two equal springs](../../../../normal-modes-of-three-masses-connected-by-two-equal-springs.md):

$$
\boxed{\begin{array}{c|c}
\mathbf a&\omega^2\\\hline
(1,1,1)&0\\
(1,0,-1)&k/m\\
(1,-2m/M,1)&k/m+2k/M
\end{array}}
$$

These three independent [eigenvectors](../../../../eigenvector.md) exhaust the three-dimensional system. The ordinary [frequencies](../../../../frequency.md) are $\omega/(2\pi)$; the values $\omega$ above are [angular frequencies](../../../../angular-frequency.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [9](../../9.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

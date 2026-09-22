<h1 id="11/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $\boldsymbol x=q e^{i\omega t}$ in [solution](../a/solution.md). The [normal mode](../../../../normal-mode.md) equation is $Aq=\lambda q$, with $\lambda=m\omega^2/k$. Its [characteristic polynomial](../../../../characteristic-polynomial.md) is

$$
\det(A-\lambda I)=(2-\lambda)\big[(2-\lambda)^2-2\big].
$$

The three [eigenvalues](../../../../eigenvalue.md) are $2-\sqrt2$, $2$, and $2+\sqrt2$. Solving the corresponding linear equations yields

$$
\boxed{\begin{array}{c|c|c}
\text{mode}&\omega&\text{mode shape }q\\\hline
1&\sqrt{(2-\sqrt2)k/m}&(1,\sqrt2,1)^T\\
2&\sqrt{2k/m}&(1,0,-1)^T\\
3&\sqrt{(2+\sqrt2)k/m}&(1,-\sqrt2,1)^T
\end{array}}
$$

Each [mode shape](../../../../mode-shape.md) may be multiplied by any nonzero scalar. Their squared [Euclidean norms](../../../../euclidean-norm.md) are $4,2,4$, respectively, so unit-normalized [eigenvectors](../../../../eigenvector.md) are $q_1/2,q_2/\sqrt2,q_3/2$. They are mutually orthogonal, as expected for the real symmetric [stiffness matrix](../../../../stiffness-matrix.md) with equal [masses](../../../../mass.md).

The entries in the table are [angular frequencies](../../../../angular-frequency.md); the corresponding ordinary [frequencies](../../../../frequency.md) in cycles per unit time are $f_j=\omega_j/(2\pi)$. All three are positive because the fixed walls remove uniform translation as a free motion.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [11](../../11.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

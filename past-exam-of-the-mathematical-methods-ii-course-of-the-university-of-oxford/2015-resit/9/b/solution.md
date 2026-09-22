<h1 id="9/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The natural [normal modes](../../../../normal-mode.md) belong to the homogeneous system with both end displacements fixed at zero. Seek $\mathbf y=\mathbf a\cos\Omega t$, so

$$
\omega_0^2\begin{pmatrix}3&-1\\-1&3\end{pmatrix}\mathbf a=\Omega^2\mathbf a.
$$

The [characteristic polynomial](../../../../characteristic-polynomial.md) is $(3\omega_0^2-\Omega^2)^2-\omega_0^4=0$. The [eigenvectors](../../../../eigenvector.md) $(1,1)$ and $(1,-1)$ therefore give

$$
\boxed{\Omega_+=\sqrt2\,\omega_0,\quad y_1=y_2;\qquad\Omega_-=2\omega_0,\quad y_1=-y_2}.
$$

The symmetric mode leaves the middle segment horizontal, while the antisymmetric mode bends it strongly and has the higher restoring stiffness. Defining $q_+=(y_1+y_2)/2$ and $q_-=(y_1-y_2)/2$ diagonalizes the driven equations too:

$$
\ddot q_++2\omega_0^2q_+=\omega_0^2h(t),\qquad\ddot q_-+4\omega_0^2q_-=-\omega_0^2h(t).
$$

This shows that the boundary drive excites both natural modes; neither natural [resonance](../../../../resonance.md) is removed by a zero drive projection.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [9](../../9.md)
3. [2015 resit](../../../2015-resit-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

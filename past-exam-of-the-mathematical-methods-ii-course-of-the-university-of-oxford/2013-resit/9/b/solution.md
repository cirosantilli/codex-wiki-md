<h1 id="9/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set the support displacement to zero and seek a [normal mode](../../../../normal-mode.md) $\mathbf x=(A,B)^{\mathsf T}\cos(\omega t+\varphi)$. With $s=m\omega^2/k$, the [generalized eigenvalue problem](../../../../generalized-eigenvalue-problem.md) requires

$$
\det\begin{pmatrix}3-s&-2\\-2&2-2s\end{pmatrix}=2(s^2-4s+1)=0.
$$

Thus

$$
\boxed{\omega_\pm^2=\frac km(2\pm\sqrt3),\qquad f_\pm=\frac1{2\pi}\sqrt{\frac km(2\pm\sqrt3)}.}
$$

The second row gives $A=(1-s)B$. The signed displacement ratios are therefore

$$
\boxed{\left(\frac{x_1}{x_2}\right)_{\rm slow}=\sqrt3-1,\qquad\left(\frac{x_1}{x_2}\right)_{\rm fast}=-1-\sqrt3.}
$$

The slow mode is in phase and the fast mode out of phase. Keeping the unequal mass matrix is essential: replacing it by the identity changes the eigenfrequencies.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [9](../../9.md)
3. [2013 resit](../../../2013-resit-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

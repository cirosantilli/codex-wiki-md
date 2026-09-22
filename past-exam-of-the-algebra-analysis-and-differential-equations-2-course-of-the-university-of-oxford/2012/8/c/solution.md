<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The same [variation of parameters](../../../../variation-of-parameters.md) construction works on $[0,\pi]$. All solutions satisfying the [boundary condition](../../../../boundary-condition.md) at zero have the form

$$
y(x)=e^{-2x}\left[C\sin x+\int_0^xe^{2t}\sin(x-t)f(t)\,dt\right].
$$

At $x=\pi$, the homogeneous term vanishes for every $C$; it can no longer be chosen to correct the final boundary value. Since $\sin(\pi-t)=\sin t$, that boundary value is zero exactly when

$$
\boxed{\int_0^\pi e^{2t}\sin t\,f(t)\,dt=0.}
$$

This condition is necessary by the displayed general solution, and sufficient by the same formula. When it holds, the full answer is

$$
\boxed{y(x)=e^{-2x}\left[C\sin x+\int_0^xe^{2t}\sin(x-t)f(t)\,dt\right],\qquad C\in\mathbb R.}
$$

For complex-valued forcing, allow $C\in\mathbb C$ instead. The freedom is addition of the nonzero homogeneous Dirichlet solution $e^{-2x}\sin x$. At this endpoint separation, the homogeneous boundary problem has a nonzero solution. The resulting [Fredholm solvability condition](../../../../fredholm-solvability-condition.md) restricts the forcing to the compatible functions described above. In the language of the [Fredholm alternative](../../../../fredholm-alternative.md), the condition is orthogonality to the adjoint null solution $e^{2x}\sin x$ of $D^2-4D+5$ with zero endpoint values.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [8](../../8.md)
3. [2012](../../../2012-split.md)
4. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

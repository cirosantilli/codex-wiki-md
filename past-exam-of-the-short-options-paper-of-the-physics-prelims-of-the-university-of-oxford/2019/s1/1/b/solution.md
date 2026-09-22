<h1 id="s1/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $A=x^2-y^2$ and $B=2xy$. Direct [differentiation](../../../../../differentiation.md) gives

$$
u_{xx}=e^{-B}[(4y^2-4x^2)\sin A+(2-8xy)\cos A],\qquad
u_{yy}=e^{-B}[(4x^2-4y^2)\sin A+(8xy-2)\cos A].
$$

Their sum vanishes, proving that $u$ is a [harmonic function](../../../../../harmonic-function.md). More generally the [Cauchy-Riemann equations](../../../../../cauchy-riemann-equations.md) give $u_{xx}+u_{yy}=v_{yx}-v_{xy}=0$ and $v_{xx}+v_{yy}=-u_{yx}+u_{xy}=0$; the [mixed partial derivatives](../../../../../mixed-partial-derivative.md) commute because a [holomorphic function](../../../../../holomorphic-function-split.md) is smooth. Since $e^{iz^2}=e^{-B}(\cos A+i\sin A)$, a [harmonic conjugate](../../../../../harmonic-conjugate.md) and the resulting [holomorphic function](../../../../../holomorphic-function-split.md) are

$$
\boxed{v=-e^{-2xy}\cos(x^2-y^2)+C,\qquad f(z)=-ie^{iz^2}+iC,\quad C\in\mathbb R.}
$$

These expressions also verify the [Cauchy-Riemann equations](../../../../../cauchy-riemann-equations.md) directly.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [S1](../../../s1.md)
4. [2019](../../../../2019-split.md)
5. [Past exam of the short options paper of the physics Prelims of the University of Oxford](../../../../split.md)
6. [Short options paper of the physics Prelims of the University of Oxford](../../../../../short-options-paper-of-the-physics-prelims-of-the-university-of-oxford.md)
7. [Year 1 of the physics course of the University of Oxford](../../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

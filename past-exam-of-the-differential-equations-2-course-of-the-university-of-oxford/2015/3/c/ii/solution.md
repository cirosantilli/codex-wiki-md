<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose the real leading [eigenfunction](../../../../../eigenfunction.md) $y_1=C\sin x$, keeping its amplitude $C\ne0$ fixed. At first order in the [regular perturbation](../../../../../regular-perturbation.md) expansion, the equation becomes

$$
y_{11}''+y_{11}=-\lambda_{11}y_1-y_1^2,\qquad y_{11}(0)=y_{11}(\pi)=0.
$$

The operator $L=D^2+1$ with these homogeneous [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) is [self-adjoint](../../../../../self-adjoint-operator.md), as allowed in the question, and its [null space](../../../../../kernel-of-a-linear-map-split.md) is spanned by $y_1$. The [Fredholm solvability condition](../../../../../fredholm-solvability-condition.md) requires the forcing to be [orthogonal](../../../../../orthogonal-vectors.md) to that [null space](../../../../../kernel-of-a-linear-map-split.md):

$$
0=\int_0^\pi y_1\bigl(-\lambda_{11}y_1-y_1^2\bigr)\,dx.
$$

The same condition follows directly by integrating $y_1Ly_{11}$ by parts: the endpoint term $[y_1y_{11}'-y_1'y_{11}]_0^\pi$ vanishes, and $Ly_1=0$. Since a nonzero real $y_1$ has a positive squared [integral](../../../../../integral-split.md),

$$
\boxed{\lambda_{11}=-\frac{\displaystyle\int_0^\pi y_1(x)^3\,dx}{\displaystyle\int_0^\pi y_1(x)^2\,dx}.}
$$

This is the requested expression and is an instance of the [leading nonlinear eigenvalue shift in a Sturm-Liouville problem](../../../../../leading-nonlinear-eigenvalue-shift-in-a-sturm-liouville-problem.md). In the amplitude convention above, $\int_0^\pi\sin^2x\,dx=\pi/2$ and $\int_0^\pi\sin^3x\,dx=4/3$, so $\lambda_{11}=-8C/(3\pi)$. For the particular choice $C=1$, it is $-8/(3\pi)$.

The [amplitude dependence of a nonlinear eigenvalue correction](../../../../../amplitude-dependence-of-a-nonlinear-eigenvalue-correction.md) follows here from the quadratic term: rescaling the [eigenfunction](../../../../../eigenfunction.md) changes the [eigenvalue](../../../../../eigenvalue.md) shift. There is no single numerical correction independent of the chosen leading amplitude. Once the [solvability condition](../../../../../solvability-condition.md) is met, $y_{11}$ is determined up to addition of a multiple of $y_1$; a normalization such as $\int_0^\pi y_1y_{11}\,dx=0$ can fix that remaining freedom.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the differential equations 2 course of the University of Oxford](../../../../split.md)
6. [Differential equations 2 course of the University of Oxford](../../../../../differential-equations-2-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

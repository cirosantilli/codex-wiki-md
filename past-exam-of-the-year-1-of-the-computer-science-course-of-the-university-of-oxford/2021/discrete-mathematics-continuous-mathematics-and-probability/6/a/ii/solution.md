<h1 id="6/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Differentiate the column [gradient](../../../../../../gradient.md) $2e^{r^Tr}r$. The [Jacobian matrix](../../../../../../jacobian-matrix.md) product rule gives one term from differentiating the scalar [exponential function](../../../../../../exponential-function.md) and one from differentiating $r$, whose [Jacobian matrix](../../../../../../jacobian-matrix.md) is the [identity matrix](../../../../../../identity-matrix.md):

$$
\boxed{H_f(x)=e^{\|r\|^2}(4rr^T+2I).}
$$

In particular, for any nonzero [vector](../../../../../../vector.md) $v$,

$$
v^TH_f(x)v=e^{\|r\|^2}\bigl(4(r^Tv)^2+2\|v\|^2\bigr)>0.
$$

Thus the [Hessian matrix](../../../../../../hessian-matrix.md) is positive definite everywhere. This calculation proves strict [convexity](../../../../../../convex-function.md) and supplies the [derivatives](../../../../../../derivative.md) needed for sums of these terms.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [6](../../../6.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)

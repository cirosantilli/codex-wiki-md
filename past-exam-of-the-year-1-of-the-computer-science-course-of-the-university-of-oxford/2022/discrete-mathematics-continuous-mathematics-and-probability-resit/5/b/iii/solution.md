<h1 id="5/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [matrix](../../../../../../matrix.md) $C=A-bb^T$ is an [invertible matrix](../../../../../../invertible-matrix.md). Indeed, on the line spanned by $b$ it has [eigenvalue](../../../../../../eigenvalue.md) $-1/2$, and on $b^\perp$ it agrees with the positive-definite restriction of $A$. Therefore the full [Newton step](../../../../../../newton-step.md) is well defined and gives

$$
\boxed{x_1=x_0-(2C)^{-1}(2Cx_0)=0.}
$$

This is the unique [stationary point](../../../../../../stationary-point.md) because $C$ is an [invertible matrix](../../../../../../invertible-matrix.md). The algebra applies to every starting point, but it does not make the answer a minimum: for $d\geq2$ it is the [saddle point](../../../../../../saddle-point.md) just classified, and for $d=1$ it is a maximum. A safeguarded minimization algorithm that replaces an [indefinite matrix](../../../../../../indefinite-matrix.md) used as its [Hessian matrix](../../../../../../hessian-matrix.md) or damps the step need not take this exact step; the assertion concerns the ordinary full [Newton step](../../../../../../newton-step.md) formula.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Discrete mathematics, continuous mathematics and probability resit](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)

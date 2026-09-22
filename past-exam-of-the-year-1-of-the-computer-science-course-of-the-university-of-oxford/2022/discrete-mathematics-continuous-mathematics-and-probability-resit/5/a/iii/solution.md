<h1 id="5/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The full, undamped [Newton's method in optimization](../../../../../../newton-s-method-in-optimization.md) step is

$$
x_1=x_0-H_f(x_0)^{-1}\nabla f(x_0)
=x_0-(2A)^{-1}(2Ax_0+b)
=-\tfrac12A^{-1}b.
$$

The [eigenvector](../../../../../../eigenvector.md) identity gives $A^{-1}b=2b$. Consequently **$x_1=-b$ for every starting point**. This is a [one-step Newton solution of a quadratic stationary equation](../../../../../../one-step-newton-solution-of-a-quadratic-stationary-equation.md): its [gradient](../../../../../../gradient.md) is an [affine function](../../../../../../affine-function.md), so a single exact Newton solve resolves it completely.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
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

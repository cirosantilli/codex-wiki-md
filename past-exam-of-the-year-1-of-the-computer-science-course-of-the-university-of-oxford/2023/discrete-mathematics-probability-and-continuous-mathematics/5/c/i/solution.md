<h1 id="5/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use [bisection](../../../../../../bisection-method.md) on $f'$ when the [derivative](../../../../../../derivative.md) is cheap and a bracket $f'(a)<0<f'(b)$ is easy to obtain. For a differentiable [convex function](../../../../../../convex-function.md), $f'$ is nondecreasing, so such a bracket locates a global [minimum](../../../../../../minimum-of-a-subset-of-a-total-order.md), allowing a flat minimizing interval. Without [convexity](../../../../../../convex-function.md), first isolate a region containing the desired local [minimum](../../../../../../minimum-of-a-subset-of-a-total-order.md); arbitrary stationary points need not be minima.

Use [golden-section search](../../../../../../golden-section-search.md) when reliable [function](../../../../../../function-split.md) values are available but [derivatives](../../../../../../derivative.md) are unavailable or expensive. It needs a bracket on which the objective is a [unimodal function](../../../../../../unimodal-function.md), commonly found by three ordered points whose middle value is below the two outer values. Those inequalities alone do not prove that the objective is a [unimodal function](../../../../../../unimodal-function.md). A [convex function](../../../../../../convex-function.md) supplies the needed shape; for a nonconvex objective, isolate an interval on which it is a [unimodal function](../../../../../../unimodal-function.md).

Both methods have [linear convergence](../../../../../../linear-convergence.md) of bracket width. [Bisection](../../../../../../bisection-method.md) contracts the width by $1/2$ per new derivative evaluation. [Golden-section search](../../../../../../golden-section-search.md) contracts it by $(\sqrt5-1)/2\approx0.618$ per new function evaluation after initialization, reusing one earlier value. Choose by evaluation cost and bracket availability as well as this contraction factor: comparing iteration counts alone can misidentify the faster method.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [5](../../../5.md)
4. [Discrete mathematics, probability and continuous mathematics](../../../../discrete-mathematics-probability-and-continuous-mathematics-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)

<h1 id="b/4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [descent direction](../../../../../descent-direction.md) $s$ satisfies $g^Ts<0$, where $g=\nabla f(x)$; the first-order [Taylor expansion](../../../../../taylor-expansion.md) then gives $f(x+\alpha s)<f(x)$ for sufficiently small $\alpha>0$. To compare directions one must fix their scale. Among Euclidean unit vectors, the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives

$$
g^Td\geq-\|g\|_2,\qquad\boxed{d=-g/\|g\|_2}\quad(g\ne0).
$$

This is the unit [steepest descent direction](../../../../../steepest-descent-direction.md). The conventional unnormalized direction used in the algorithm is the same ray, $\boxed{s=-g}$. Equivalently it is the unique minimizer of $g^Ts+\tfrac12\|s\|_2^2=\tfrac12\|s+g\|_2^2-\tfrac12\|g\|_2^2$. If $g=0$ there is no strict first-order [descent direction](../../../../../descent-direction.md), and the conventional update is zero.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

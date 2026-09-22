<h1 id="7/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Set $D(s)=4-2s-s^2$, so $D(s)G(s)=s^2$. Differentiate once and evaluate at $s=1$, using $D(1)=1$, $D'(1)=-4$, $G(1)=1$:

$$
-4+G'(1)=2,\qquad G'(1)=6.
$$

A second differentiation gives $D''G+2D'G'+DG''=2$, hence

$$
-2-8\cdot6+G''(1)=2,\qquad G''(1)=52.
$$

The derivatives of a [probability generating function](../../../../../../probability-generating-function.md) give $G'(1)=\mathbb E[F]$ and $G''(1)=\mathbb E[F(F-1)]$. Consequently **$\operatorname{Var}(F)=52+6-6^2=22$**. The earlier [geometric tail bound from a uniform escape probability](../../../../../../geometric-tail-bound-from-a-uniform-escape-probability.md) ensures the needed [moments](../../../../../../moment.md) are finite.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Discrete mathematics, continuous mathematics, and probability resit](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)

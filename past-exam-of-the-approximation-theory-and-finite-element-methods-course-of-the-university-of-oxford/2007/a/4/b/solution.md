<h1 id="a/4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [Taylor expansion](../../../../../taylor-expansion.md) $\sqrt{1-x}=1-x/2-x^2/8+O(x^3)$. Expanding the rational form gives

$$
\frac{a_0+a_1x}{1+b_1x}
=a_0+(a_1-a_0b_1)x+(a_0b_1^2-a_1b_1)x^2+O(x^3).
$$

Matching through degree two yields $a_0=1$, $a_1-b_1=-1/2$, and $b_1^2-a_1b_1=-1/8$. The last equation becomes $b_1/2=-1/8$, so

$$
\boxed{a_0=1,\qquad a_1=-\frac34,\qquad b_1=-\frac14,
\quad r(x)=\frac{1-3x/4}{1-x/4}.}
$$

This is the $[1/1]$ Padé approximant about zero. Its pole is at four, outside the [interpolation](../../../../../interpolation-split.md) interval; its order of matching is local and does not assert uniform minimax optimality.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [4](../../4.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

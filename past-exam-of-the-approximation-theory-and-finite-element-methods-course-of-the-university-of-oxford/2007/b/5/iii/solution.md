<h1 id="b/5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The weak equation implies $u''=x^2u-f\in L^2(a,b)$ in [distributions](../../../../../distribution-mathematical-analysis.md), hence $u\in H^2(a,b)$. Its nodal interpolant satisfies

$$
\|(u-I_hu)'\|_2\leq\frac h\pi\|u''\|_2,\qquad
\|u-I_hu\|_2\leq\frac{h^2}{\pi^2}\|u''\|_2.
$$

These follow interval by interval: the [interpolation](../../../../../interpolation-split.md) error vanishes at both endpoints, and its [derivative](../../../../../derivative.md) has mean zero, so two Poincaré inequalities apply. If $M$ and $\gamma$ are the continuity and [coercivity](../../../../../coercive-function.md) constants, [Céa's lemma](../../../../../cea-s-lemma.md) gives

$$
\|u-u_h\|_{H^1}\leq\frac M\gamma\|u-I_hu\|_{H^1}
\leq\frac M\gamma\sqrt{\frac{h^2}{\pi^2}+\frac{h^4}{\pi^4}}\,\|u''\|_2
=\boxed{O(h)}.
$$

All constants are independent of the mesh size.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [B](../../../b.md)
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

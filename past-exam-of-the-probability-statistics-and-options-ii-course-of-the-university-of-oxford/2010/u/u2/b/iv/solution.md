<h1 id="u/u2/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

At $x=1$, the [derivative](../../../../../../derivative.md) and [curvature](../../../../../../second-derivative.md) are $f'(1)=8$, $f''(1)=-8$, so the next iterate is $2$. At $x=2$, they are $f'(2)=4$, $f''(2)=4$, so the next iterate is $1$. Hence

$$
\boxed{1\longmapsto2\longmapsto1\longmapsto2\longmapsto\cdots.}
$$

The undamped [algorithm](../../../../../../algorithm-split.md) does not converge to a [minimum](../../../../../../local-minimum.md); it has an exact [two-cycle](../../../../../../period-two-orbit.md). The implementation in (iii) detects this after returning to one and reports failure. This example illustrates why the local convergence result in (ii) does not justify global success.

## ↑ Ancestors (14)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [U2](../../../u2.md)
4. [U](../../../../u.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../../split.md)
7. [Probability, statistics and options II course of the University of Oxford](../../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Mathematics and statistics course of the University of Oxford](../../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)

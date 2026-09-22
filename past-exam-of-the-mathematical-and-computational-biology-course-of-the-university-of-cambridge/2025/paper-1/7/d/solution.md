<h1 id="7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Expanding the squared [Euclidean distances](../../../../../euclidean-distance.md) gives

$$
\|x-z_1\|^2-\|x-z_2\|^2
=-2x^{\mathsf T}(z_1-z_2)+\|z_1\|^2-\|z_2\|^2.
$$

For distinct [centroids](../../../../../centroid.md), choose

$$
\boxed{w=2(z_1-z_2),\qquad b=\|z_2\|^2-\|z_1\|^2}.
$$

A point assigned to $C_1$ has the displayed distance difference at most zero and therefore $w^{\mathsf T}x+b\ge0$; assignment to $C_2$ gives the reverse inequality. The separating [hyperplane](../../../../../hyperplane.md) is the [perpendicular bisector](../../../../../perpendicular-bisector.md) of the line segment joining the two [centroids](../../../../../centroid.md). Points tied between them lie on that [hyperplane](../../../../../hyperplane.md). This is the [nearest-centroid decision hyperplane](../../../../../nearest-centroid-decision-hyperplane.md).

The requested nonzero $w$ needs the additional assumption $z_1\ne z_2$. It does not follow from the stated algorithm alone. In one dimension, take $C_1=\{-1,1\}$ and $C_2=\{0\}$, whose [centroids](../../../../../centroid.md) are both zero. A tie rule that retains previous assignments can leave this configuration after an iteration. The inequalities at $-1,1$ imply $b\ge|w|$, while the inequality at zero implies $b\le0$, forcing $w=0$. Thus the unconditional nonzero-separator claim has this degenerate exception.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [7](../../7.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

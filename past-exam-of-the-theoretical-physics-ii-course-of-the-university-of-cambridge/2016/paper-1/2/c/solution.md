<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [matrix](../../../../../matrix.md) $R$ belongs to the [special orthogonal group](../../../../../special-orthogonal-group.md) in four dimensions precisely when

$$
\boxed{R\in M_4(\mathbb R),\qquad R^{\mathsf T}R=I,\qquad\det R=1.}
$$

Differentiating the [orthogonality](../../../../../orthogonal-vectors.md) relation along a path $R(\epsilon)=I+\epsilon X+O(\epsilon^2)$ gives $X^{\mathsf T}+X=0$. Thus its [Lie algebra](../../../../../lie-algebra-split.md) consists of real antisymmetric four-by-four [matrices](../../../../../matrix.md). Such a [matrix](../../../../../matrix.md) has one free entry for each unordered coordinate pair, giving dimension $\binom42=6$.

Each displayed generator has a single two-coordinate antisymmetric block. The $K$ [matrices](../../../../../matrix.md) cover planes $(1,2),(1,3),(1,4)$; the $L$ [matrices](../../../../../matrix.md) cover $(3,4),(2,4),(2,3)$, with their printed orientations. These are all six distinct planes. Therefore the generators are linearly independent and span the full antisymmetric space: **they form a basis of $\mathfrak{so}(4)$**.

Conversely, exponentiating any real antisymmetric $X$ gives $(e^X)^{\mathsf T}e^X=I$ and $\det(e^X)=e^{\operatorname{tr}X}=1$. This verifies that the infinitesimal [matrices](../../../../../matrix.md) generate proper rotations rather than reflections.

## ↑ Ancestors (15)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the theoretical physics II course of the University of Cambridge](../../../../split.md)
6. [Theoretical Physics II course of the University of Cambridge](../../../../../theoretical-physics-ii-course-of-the-university-of-cambridge.md)
7. [Theoretical Physics course of the University of Cambridge](../../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../split.md)

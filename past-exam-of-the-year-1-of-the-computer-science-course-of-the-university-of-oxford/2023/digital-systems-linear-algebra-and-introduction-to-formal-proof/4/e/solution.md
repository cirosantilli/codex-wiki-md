<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Both $L$ and $R$ have $m$ [linearly independent](../../../../../linear-independence.md) columns. The [Gram matrix](../../../../../gram-matrix.md) $R^\top R$ is invertible because

$$
y^\top R^\top Ry=\|Ry\|^2>0\qquad(y\ne0).
$$

Consequently $R^\top$ is a [surjective linear map](../../../../../surjective-linear-map.md): for any $y\in\mathbb R^m$, the choice $x=R(R^\top R)^{-1}y$ satisfies $R^\top x=y$. Hence

$$
\operatorname{im}B=L(\operatorname{im}R^\top)=\operatorname{im}L.
$$

The latter [image of a linear map](../../../../../image-of-a-linear-map.md) has [dimension](../../../../../dimension-vector-space.md) $m$, giving **$\operatorname{rank}B=m$**. If $m=0$, $B=0$ and the conclusion is immediate. This argument explains why the product retains its full possible [matrix rank](../../../../../matrix-rank.md); a general product of two [matrices](../../../../../matrix.md) need not do so.

## ↑ Ancestors (13)

1. [E](../e.md)
2. [4](../../4.md)
3. [Linear algebra](../../linear-algebra.md)
4. [Digital systems, linear algebra and introduction to formal proof](../../../digital-systems-linear-algebra-and-introduction-to-formal-proof-split.md)
5. [2023](../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

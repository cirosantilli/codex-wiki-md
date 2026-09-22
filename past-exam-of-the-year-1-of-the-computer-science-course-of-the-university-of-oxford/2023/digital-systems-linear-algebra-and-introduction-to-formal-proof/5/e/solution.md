<h1 id="5/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The [dimensions](../../../../../dimension-vector-space.md) of the nested [images of a linear map](../../../../../image-of-a-linear-map.md)

$$
V=\mathcal R(h^0)\supseteq\mathcal R(h)\supseteq\cdots
$$

can strictly decrease at most $n$ times. If all the first $n$ inclusions are strict, $\mathcal R(h^n)=0$ and is stable. Otherwise an earlier equality occurs and (d) makes every subsequent image equal. Thus in all cases

$$
\mathcal R(h^n)=\mathcal R(h^{2n}).
$$

By the [rank-nullity theorem](../../../../../rank-nullity-theorem.md) and inclusion of the [null spaces](../../../../../kernel-of-a-linear-map-split.md), this also gives $\ker h^n=\ker h^{2n}$. If $v\in\mathcal R(h^n)\cap\ker h^n$, write $v=h^nu$. Then $0=h^nv=h^{2n}u$, so $u\in\ker h^{2n}=\ker h^n$ and $v=0$. Hence the [intersection](../../../../../set-intersection.md) is zero. Finally the [rank-nullity theorem](../../../../../rank-nullity-theorem.md) gives

$$
\dim\mathcal R(h^n)+\dim\ker h^n=n.
$$

Zero [intersection](../../../../../set-intersection.md) and this [dimension](../../../../../dimension-vector-space.md) sum prove

$$
\boxed{V=\mathcal R(h^n)\oplus\mathcal N(h^n).}
$$

This is the [finite-dimensional Fitting decomposition](../../../../../finite-dimensional-fitting-decomposition.md). It includes the zero-dimensional case, for which $V=0$ and the assertion is immediate.

## ↑ Ancestors (13)

1. [E](../e.md)
2. [5](../../5.md)
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

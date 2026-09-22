<h1 id="5/a/ii/solution">Solution</h1>

↑ **Parent:** [ii](../ii.md)

Parametrize the [matrices](../../../../../../../matrix.md) by

$$
h(a,b,c)=\begin{pmatrix}1&a&b\\0&1&c\\0&0&1\end{pmatrix},
\qquad a,b,c\in\mathbb Z_3.
$$

Direct [matrix multiplication](../../../../../../../matrix-multiplication.md) gives

$$
h(a,b,c)h(a',b',c')
=h(a+a',\ b+b'+ac',\ c+c').
$$

This proves closure. The [identity matrix](../../../../../../../identity-matrix.md) is $h(0,0,0)$, and the formula

$$
\boxed{h(a,b,c)^{-1}=h(-a,\ ac-b,\ -c)}
$$

gives both a left and a right inverse, as substitution in the product formula verifies. Thus each element is an [invertible matrix](../../../../../../../invertible-matrix.md), and the [subgroup test](../../../../../../../subgroup-test.md) shows that $H$ is a [subgroup](../../../../../../../subgroup.md) of $\operatorname{GL}_3(\mathbb Z_3)$. It is the [unitriangular group](../../../../../../../unitriangular-group.md) $\operatorname{UT}_3(\mathbb F_3)$ and has $3^3=27$ elements.

## ↑ Ancestors (13)

1. [ii](../ii.md)
2. [a](../../a.md)
3. [5](../../../5.md)
4. [Mathematics I](../../../../mathematics-i-split.md)
5. [Prelims](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)

<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the convention that the [inner product](../../../../../inner-product-split.md) is conjugate-linear in its first argument and linear in its second, as in part (b). The [adjoint operator](../../../../../adjoint-operator.md) is characterized by

$$
\boxed{\langle Tv,w\rangle=\langle v,T^*w\rangle
\qquad(v,w\in V).}
$$

Existence and uniqueness follow from the finite-dimensional representation of [linear functionals](../../../../../linear-functional.md) by the [inner product](../../../../../inner-product-split.md). More concretely, choose an [orthonormal basis](../../../../../orthonormal-basis.md) $e_i$ and let $a_{ij}=\langle e_i,Te_j\rangle$. Then

$$
\langle e_i,T^*e_j\rangle=\langle Te_i,e_j\rangle
=\overline{a_{ji}},
$$

which defines $T^*$ uniquely and verifies the required identity by expansion in that [basis](../../../../../basis.md). Thus its [matrix](../../../../../matrix.md) is the conjugate transpose, proved here rather than assumed. A [self-adjoint operator](../../../../../self-adjoint-operator.md) satisfies $T^*=T$, equivalently $\langle Tv,w\rangle=\langle v,Tw\rangle$ for every pair of vectors.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the linear algebra course of the University of Oxford](../../../../split.md)
6. [Linear algebra course of the University of Oxford](../../../../../linear-algebra-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

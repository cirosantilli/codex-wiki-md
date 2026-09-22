<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Split $f=f_-+a_0+f_+$ into strictly negative and strictly positive Fourier parts, and let $A=T(f_-)$, $B=T(f_+)$. The Toeplitz multiplication rule is $T(g)T(h)=T(gh)$ when $g$ is coanalytic or $h$ is analytic. It follows directly because the discarded negative Fourier part cannot return to the Hardy space in those cases. Thus exponentiation within either subalgebra is exact, and

$$
T(e^f)T(e^{-f})=e^Ae^Be^{-A}e^{-B}.
$$

The constant terms cancel. If $S=T(z)$ is the unilateral shift, $A=\sum_{m>0}a_{-m}(S^*)^m$ and $B=\sum_{n>0}a_nS^n$. The [commutator](../../../../../../commutator.md) $[(S^*)^m,S^n]$ is finite [rank](../../../../../../rank-one-quadratic-form.md), with [trace](../../../../../../matrix-trace.md) $n$ when $m=n$ and zero otherwise. For equal powers it is the projection onto the first $n$ basis [vectors](../../../../../../vector.md); for unequal powers its [matrix](../../../../../../matrix.md) has no diagonal entries. Its [trace norm](../../../../../../trace-norm.md) is bounded by $2\min(m,n)$. Smoothness of $f$ makes the weighted double coefficient sum finite, so the [commutator](../../../../../../commutator.md) [series](../../../../../../series-mathematics.md) converges in [trace norm](../../../../../../trace-norm.md) and

$$
\operatorname{Tr}[A,B]=\sum_{n>0}n a_na_{-n}.
$$

Applying part (c) proves the [Toeplitz exponential determinant identity](../../../../../../toeplitz-exponential-determinant-identity.md)

$$
\boxed{\det(T(e^f)T(e^{-f}))=\exp\left(\sum_{n>0}na_na_{-n}\right).}
$$

In particular the product is an invertible identity-plus-trace-class operator, so the [determinant](../../../../../../determinant.md) in the formula is well-defined.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 10](../../../paper-10-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

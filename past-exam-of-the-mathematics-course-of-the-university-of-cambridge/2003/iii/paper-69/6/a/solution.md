<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume the [spline knot sequence](../../../../../../spline-knot-sequence.md) is ordered and its relevant support spans satisfy $t_{i+k}>t_i$. For distinct knots, the [divided difference](../../../../../../divided-difference.md) is a finite linear combination of evaluations, so it commutes with integration. With $u\in[a,b]$,

$$
\int_a^b(u-t)_+^{k-1}\,dt=\int_a^u(u-t)^{k-1}\,dt=\frac{(u-a)^k}{k}.
$$

Taking the order-$k$ [divided difference](../../../../../../divided-difference.md) in $u$ gives

$$
\boxed{\int_a^bM_i(t)\,dt=k[t_i,\ldots,t_{i+k}]\frac{(u-a)^k}{k}=1}.
$$

Indeed, the order-$k$ [divided difference](../../../../../../divided-difference.md) of a degree-$k$ [polynomial](../../../../../../polynomial-split.md) is its [leading coefficient](../../../../../../leading-coefficient-of-a-polynomial.md), here $1/k$. This proves the [unit-integral normalization of a B-spline](../../../../../../unit-integral-normalization-of-a-b-spline.md). Admissible repeated knots follow by coalescing knots, with the usual one-sided endpoint conventions.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

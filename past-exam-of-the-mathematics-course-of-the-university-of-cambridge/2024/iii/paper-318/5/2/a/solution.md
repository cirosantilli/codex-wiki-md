<h1 id="5/2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The integral form of the [Taylor theorem](../../../../../../../taylor-theorem.md) about the left endpoint is

$$
f(x)=q_{k-1}(x)+\frac1{(k-1)!}
\int_a^b(x-t)_+^{k-1}f^{(k)}(t)\,dt,
$$

where $q_{k-1}\in\mathcal P_{k-1}$. Apply the order-$k$ [divided difference](../../../../../../../divided-difference.md) at $x_i,\ldots,x_{i+k}$. The polynomial term vanishes, and linearity permits interchange with the integral:

$$
f[x_i,\ldots,x_{i+k}]
=\frac1{(k-1)!}\int_a^b
[x_i,\ldots,x_{i+k}](\mathord\cdot-t)_+^{k-1}
f^{(k)}(t)\,dt.
$$

By the definition $M_i(t)=k[x_i,\ldots,x_{i+k}](\mathord\cdot-t)_+^{k-1}$,

$$
\boxed{f[x_i,\ldots,x_{i+k}]
=\frac1{k!}\int_a^bM_i(t)f^{(k)}(t)\,dt}.
$$

This is the [Peano kernel theorem](../../../../../../../peano-kernel-theorem.md) for the divided-difference functional.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [5](../../../5.md)
4. [Paper 318](../../../../paper-318-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

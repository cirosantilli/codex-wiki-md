<h1 id="12f/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $L=\limsup_{n\to\infty}|a_n|^{1/n}$. The [Cauchy-Hadamard theorem](../../../../../../../cauchy-hadamard-theorem.md), proved by applying the root test, gives a [radius of convergence](../../../../../../../radius-of-convergence.md)

$$
R=\frac1L
$$

with the usual conventions. For $|z|<R$, choose $q<1$ eventually bounding $|a_nz^n|^{1/n}$, which gives absolute convergence by comparison with a geometric series. For $|z|>R$, infinitely many terms have $n$th root greater than one, so the terms fail to tend to zero and the series diverges.

Here $R=2$ and the assumed limit gives $|a_n|^{1/n}\to1/2$. Therefore

$$
|a_{kn}|^{1/n}
=\left(|a_{kn}|^{1/(kn)}\right)^k
\longrightarrow2^{-k}.
$$

Thus

$$
\boxed{\sum_{n=0}^\infty a_{kn}z^n
\text{ has radius }2^k}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [12F](../../../12f.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ia](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

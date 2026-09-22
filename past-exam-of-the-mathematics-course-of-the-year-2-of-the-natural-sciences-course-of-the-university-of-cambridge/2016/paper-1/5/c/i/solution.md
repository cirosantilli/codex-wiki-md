<h1 id="5/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

First, $I-A$ is invertible. If $(I-A)x=0$ for a real [vector](../../../../../../vector.md), then $Ax=x$, whereas the [skew-symmetric matrix](../../../../../../skew-symmetric-matrix.md) identity gives $x^TAx=0$; hence $x^Tx=0$ and $x=0$. Thus its real [kernel](../../../../../../kernel-of-a-linear-map-split.md) is trivial, which suffices for invertibility. The same argument applies to $I+A$.

Using $A^T=-A$ and the rule for the [transpose](../../../../../../transpose.md) of a product,

$$
N^T=[(I-A)^{-1}]^T(I+A)^T=(I+A)^{-1}(I-A).
$$

The factors $I+A$ and $I-A$ commute, as do the required inverses. Consequently

$$
N^TN=(I+A)^{-1}(I-A)(I+A)(I-A)^{-1}=I.
$$

Thus $\boxed{N\text{ is orthogonal}}$. This is the [Cayley transform of a real skew-symmetric matrix](../../../../../../cayley-transform-of-a-real-skew-symmetric-matrix.md).

## ↑ Ancestors (14)

1. [I](../i.md)
2. [C](../../c.md)
3. [5](../../../5.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)

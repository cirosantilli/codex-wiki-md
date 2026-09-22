<h1 id="6a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [floor-half generating function](../../../../../../floor-half-generating-function.md) is

$$
H(x)=\sum_{n\geq1}\left\lfloor\frac n2\right\rfloor x^n
=\frac{x^2}{(1-x)^2(1+x)}.
$$

Summing $u_n-2u_{n-1}=\lfloor n/2\rfloor$ for $n\geq1$ gives

$$
G(x)-1-2xG(x)=H(x),
$$

so

$$
\boxed{
G(x)=\frac{1+\dfrac{x^2}{(1-x)^2(1+x)}}{1-2x}}.
$$

Since

$$
\left\lfloor\frac n2\right\rfloor
=\frac n2-\frac14+\frac14(-1)^n,
$$

a particular solution is

$$
-\frac n2-\frac34+\frac1{12}(-1)^n.
$$

Adding the homogeneous term $C2^n$ and imposing $u_0=1$ gives $C=5/3$. Therefore

$$
\boxed{
u_n=\frac53\,2^n-\frac n2-\frac34+\frac1{12}(-1)^n}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6A](../../6a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

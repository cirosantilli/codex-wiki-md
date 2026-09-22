<h1 id="6a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The homogeneous characteristic equation is

$$
r^2+r-6=(r-2)(r+3)=0.
$$

A linear particular solution $u_n=an+b$ gives

$$
-4an+11a-4b=n,
$$

so $a=-1/4$ and $b=-11/16$. Thus

$$
u_n=A2^n+B(-3)^n-\frac n4-\frac{11}{16}.
$$

The initial data yield $A=1$ and $B=-5/16$, hence

$$
\boxed{u_n=2^n-\frac5{16}(-3)^n-\frac n4-\frac{11}{16}}.
$$

For the [ordinary generating function of a recurrence](../../../../../../ordinary-generating-function-of-a-recurrence.md), multiply by $x^n$ and sum for $n\geq2$. Using $u_0=0,u_1=2$ gives

$$
(1+x-6x^2)G(x)
=x+\frac{x}{(1-x)^2}.
$$

Equivalently,

$$
\boxed{
G(x)=
\frac1{1-2x}
-\frac5{16(1+3x)}
-\frac{x}{4(1-x)^2}
-\frac{11}{16(1-x)}}.
$$

Expanding each geometric [series](../../../../../../series-mathematics.md) gives exactly the displayed formula for $u_n$, verifying consistency.

## ↑ Ancestors (11)

1. [A](../a.md)
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

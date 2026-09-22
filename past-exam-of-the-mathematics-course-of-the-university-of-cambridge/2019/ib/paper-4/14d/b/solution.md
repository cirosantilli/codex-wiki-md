<h1 id="14d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Taking the [Laplace transform](../../../../../../laplace-transform.md) in $t$ and using the initial condition $u(r,0)=u_0$, the [radial heat equation in three dimensions](../../../../../../radial-heat-equation-in-three-dimensions.md) becomes

$$
sU-u_0=\frac1r(rU)_{rr}.
$$

Put $W=rU$ and $q=\sqrt s$. Then

$$
W''-sW=-u_0r,
$$

so

$$
U(r,s)=\frac{u_0}{s}+\frac{A(s)\sinh(qr)+B(s)\cosh(qr)}r.
$$

Finiteness at the centre forces $B(s)=0$.

The transformed boundary condition is

$$
\frac1kU_r(a,s)=\frac{u_0}{s}-U(a,s)-\frac1{s^2}.
$$

Since

$$
U_r(a,s)=A(s)\frac{qa\cosh(qa)-\sinh(qa)}{a^2},
$$

substitution and cancellation of the two $u_0/s$ terms gives

$$
A(s)\left[\frac{qa\cosh(qa)-\sinh(qa)}{ka^2}+\frac{\sinh(qa)}a\right]
=-\frac1{s^2}.
$$

Hence

$$
A(s)=-\frac{ka^2}{s^2\{qa\cosh(qa)+(ka-1)\sinh(qa)\}},
$$

and the required explicit transform is

$$
\boxed{
U(r,s)=\frac{u_0}{s}
-\frac{ka^2\sinh(r\sqrt s)}
{r s^2\{a\sqrt s\cosh(a\sqrt s)+(ka-1)\sinh(a\sqrt s)\}}
}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [14D](../../14d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

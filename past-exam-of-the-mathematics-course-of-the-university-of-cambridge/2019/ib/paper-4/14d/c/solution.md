<h1 id="14d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Taking $r\to0$ and using $\sinh(r\sqrt s)/r\to\sqrt s$ gives

$$
U(0,s)=\frac{u_0}{s}
-\frac{ka^2\sqrt s}
{s^2\{a\sqrt s\cosh(a\sqrt s)+(ka-1)\sinh(a\sqrt s)\}}.
$$

Set $x=a\sqrt s$. The [Taylor series](../../../../../../taylor-series.md) of the denominator is

$$
x\cosh x+(ka-1)\sinh x
=ka\,x+\frac{ka+2}{6}x^3+O(x^5).
$$

Consequently

$$
\frac{ka^2\sqrt s}{a\sqrt s\cosh(a\sqrt s)+(ka-1)\sinh(a\sqrt s)}
=1-\left(\frac{a^2}{6}+\frac{a}{3k}\right)s+O(s^2).
$$

The singular part at $s=0$ is therefore

$$
U(0,s)=-\frac1{s^2}
+\frac1s\left(u_0+\frac{a}{3k}+\frac{a^2}{6}\right)+O(1).
$$

Using [long-time asymptotics from a Laplace transform](../../../../../../long-time-asymptotics-from-a-laplace-transform.md) and part (a), the centre temperature has late-time behaviour

$$
\boxed{u(0,t)\sim u_0-t+\frac{a}{3k}+\frac{a^2}{6}}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
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

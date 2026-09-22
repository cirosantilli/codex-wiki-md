<h1 id="37b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume $qE>0$ and put

$$
\alpha=\frac{qE}{mc}.
$$

The nonzero four-velocity equations are

$$
\dot u^0=\alpha u^x,\qquad \dot u^x=\alpha u^0,
$$

with $u^0(0)=c$ and $u^x(0)=0$. Hence

$$
u^0=c\cosh(\alpha\tau),\qquad
u^x=c\sinh(\alpha\tau).
$$

Integrating from the origin gives the uniformly accelerated trajectory

$$
\boxed{
ct=\frac c\alpha\sinh(\alpha\tau),\qquad
x=\frac c\alpha\{\cosh(\alpha\tau)-1\},\qquad y=z=0.
}
$$

The light ray has $x_L=-h+ct$. At interception, $x_L=x$, so

$$
h=ct-x=\frac c\alpha\left(1-e^{-\alpha\tau}\right).
$$

A finite solution exists exactly when

$$
h<h_c=\frac c\alpha=\frac{mc^2}{qE}.
$$

Then

$$
\tau_c=-\frac1\alpha\log\left(1-\frac{\alpha h}{c}\right),
$$

and, writing $H=\alpha h/c$,

$$
t_c=\frac1\alpha\sinh(\alpha\tau_c)
=\frac{H(2-H)}{2\alpha(1-H)}.
$$

At $h=h_c$ interception is approached only as $t\to\infty$, and for $h>h_c$ it never occurs. The limiting backward light ray is the [Rindler horizon](../../../../../../rindler-horizon.md) of the accelerated particle.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [37B](../../37b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

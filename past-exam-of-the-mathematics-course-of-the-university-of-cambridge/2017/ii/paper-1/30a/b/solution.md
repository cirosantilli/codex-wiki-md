<h1 id="30a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $k\ne0$, put $t=k^2>0$ and use the positive-definite [Lyapunov function](../../../../../../lyapunov-function.md) $V=x^2+ty^2$. Its [derivative](../../../../../../derivative.md) is

$$
\dot V=-2V+2\{x^4+\beta(1+t)x^2y^2+ty^4\}.
$$

For $V>0$ set $u=x^2/V\in[0,1]$. The brace divided by $V^2$ is $Au^2+2Bu(1-u)+C(1-u)^2$, where $A=1$, $B=\beta(1+t)/(2t)$ and $C=1/t$. Since $\beta>2$, $B>A,C$. Completing the square gives its maximum

$$
M=\frac{B^2-AC}{2B-A-C}
=\frac{\beta^2(1+t)^2-4t}{4t(1+t)(\beta-1)}.
$$

Hence $\dot V\le-2V+2MV^2$. If $V(0)<1/M$, this sublevel region is positively invariant: $V$ decreases, and $\dot V\le-2(1-MV(0))V$. The exponential bound makes $V\to0$. The trajectory is bounded in a compact ellipse, so smoothness of the [vector field](../../../../../../vector-field.md) also guarantees existence for every positive time. Therefore

$$
\boxed{x^2+k^2y^2<\frac{4k^2(1+k^2)(\beta-1)}{\beta^2(1+k^2)^2-4k^2}
\ \Longrightarrow\ (x(t),y(t))\to(0,0)}.
$$

For $k=0$ the displayed strict inequality has no solutions; negative $k$ gives the same ellipse as $-k$. Taking the union of the nonempty ellipses is valid because each point needs only one Lyapunov certificate.

At $k=1$ the certified disk has squared radius $2/(\beta+1)$. Along $y=0$, the limiting threshold as $k^2\to\infty$ is $4(\beta-1)/\beta^2$, which is strictly larger, since their difference is $2(\beta^2-2)/(\beta^2(\beta+1))>0$ for $\beta>2$. Choose $x^2$ strictly between these thresholds and then a sufficiently large finite $k$. This point is certified by that ellipse but lies outside the $k=1$ disk. Thus **the union gives a strictly larger certified region**. It need not equal the whole [basin of attraction](../../../../../../basin-of-attraction.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [30A](../../30a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

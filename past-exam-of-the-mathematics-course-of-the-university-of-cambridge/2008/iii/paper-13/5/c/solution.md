<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Work first on $B=B_1$, and let $m=|B|^{-1}\int_Bu$. Put $Z=\{u=0\}$. Since $|Z|\geq\theta|B|$,

$$
\theta|B|m^2\leq |Z|m^2=\int_Z|u-m|^2\leq\int_B|u-m|^2.
$$

Also $\int_Bu^2=\int_B|u-m|^2+|B|m^2$, so

$$
\int_Bu^2\leq(1+\theta^{-1})\int_B|u-m|^2.
$$

The [Poincare-Wirtinger inequality](../../../../../../poincare-wirtinger-inequality.md) now bounds the last integral by $C_n\int_B|Du|^2$. Here is a direct proof on the ball. For smooth $u$, the variance identity and the fundamental theorem along line segments give

$$
\int_B|u-m|^2=\frac1{2|B|}\int_B\int_B|u(x)-u(y)|^2\,dx\,dy,
$$



$$
|u(x)-u(y)|^2\leq4\int_0^1|Du((1-t)x+ty)|^2\,dt.
$$

For $0\leq t\leq1/2$, fix $y$ and change variables $z=(1-t)x+ty$. Convexity keeps $z$ inside $B$, and the inverse Jacobian is at most $2^n$. Thus the double integral of this [gradient](../../../../../../gradient.md) term is at most $2^n|B|\int_B|Du|^2$. For $1/2\leq t\leq1$, fix $x$ instead and obtain the same bound. Integration over $t$ proves $\int_B|u-m|^2\leq2^{n+1}\int_B|Du|^2$. Density of smooth functions in $W^{1,2}(B)$ passes the estimate to all Sobolev functions.

For a ball centered at $a$ with radius $R$, set $v(y)=u(a+Ry)$. Its zero set has at least the same volume fraction $\theta$, while $\int_{B_1}v^2=R^{-n}\int_{B_R}u^2$ and $\int_{B_1}|Dv|^2=R^{2-n}\int_{B_R}|Du|^2$. Therefore

$$
\boxed{\int_{B_R}u^2\leq2^{n+1}(1+\theta^{-1})R^2\int_{B_R}|Du|^2.}
$$

This establishes the [Poincare inequality with a positive-measure zero set](../../../../../../poincare-inequality-with-a-positive-measure-zero-set.md), with an explicit admissible constant. If $\theta=1$, the function is already zero [almost everywhere](../../../../../../almost-everywhere.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

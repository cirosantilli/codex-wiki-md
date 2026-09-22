<h1 id="22h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Every function with the stated two linear pieces can be written

$$
f(x)=a+bx+c\left|x-\frac12\right|
$$

for suitable real constants $a,b,c$. Since

$$
\left|x-\frac12\right|=\sqrt{\left(x-\frac12\right)^2},
$$

define

$$
Q_i(x)=a+bx+cP_i\!\left(\left(x-\frac12\right)^2\right).
$$

This is a polynomial. The argument of $P_i$ lies in $[0,1/4]\subseteq[0,1]$, so

$$
\boxed{\|Q_i-f\|_\infty
\leq |c|\sup_{u\in[0,1]}|P_i(u)-\sqrt u|
\longrightarrow0.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [22H](../../22h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

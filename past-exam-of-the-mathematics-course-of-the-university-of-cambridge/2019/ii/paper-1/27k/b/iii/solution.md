<h1 id="27k/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

First, $f(0)=1$. For every $r\geq0$,

$$
f(r)=f(r/2)^2\geq0.
$$

It cannot vanish: if $f(r_0)=0$ for some $r_0>0$, then

$$
0=f(r_0)=f(r_0/n)^n
$$

would imply $f(r_0/n)=0$ for every positive integer $n$, contradicting continuity at zero. Thus $f(r)>0$. Since every characteristic function has modulus at most one,

$$
\boxed{0<f(r)\leq1}.
$$

Now set $h(r)=-\log f(r)$. It is continuous, nonnegative, and additive:

$$
h(r_1+r_2)=h(r_1)+h(r_2).
$$

The classification of a [continuous additive function on the nonnegative real numbers](../../../../../../../continuous-additive-function-on-the-nonnegative-real-numbers.md) gives $h(r)=\alpha r$, where $\alpha=h(1)\geq0$. Consequently

$$
\boxed{f(r)=e^{-\alpha r}\qquad(r\geq0)}.
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [27K](../../../27k.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

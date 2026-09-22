<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Expand the exact solution about $t_{n+1}=t$. The unscaled [local truncation error](../../../../../../local-truncation-error.md) is

$$
\begin{aligned}
 d_h&=y(t+h)-y(t-h)-h\{a y'(t+h)+2(1-a)y'(t)+a y'(t-h)\}\\
 &=\left(\frac13-a\right)h^3y'''(t)+\left(\frac1{60}-\frac a{12}\right)h^5y^{(5)}(t)+O(h^7).
\end{aligned}
$$

Only odd powers occur in this centered expansion. Unless $a=1/3$, the first nonzero coefficient is the $h^3$ coefficient, giving [order of a numerical method](../../../../../../order-of-a-numerical-method.md) two. For $a=1/3$, that term vanishes but the next coefficient is $-1/90$, giving [order of a numerical method](../../../../../../order-of-a-numerical-method.md) four. Thus

$$
\boxed{p=2\quad(a\ne1/3),\qquad p=4\quad(a=1/3).}
$$

These are exact orders for general smooth [ordinary differential equations](../../../../../../ordinary-differential-equation.md), since the respective first surviving derivatives need not vanish. With starting errors $O(h^p)$, the [zero-stability](../../../../../../zero-stability.md) established in part (a) makes the [global error](../../../../../../global-discretization-error.md) $O(h^p)$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [Section A](../../section-a.md)
4. [Paper 68](../../../paper-68-split.md)
5. [Iii](../../../split.md)
6. [2015](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)

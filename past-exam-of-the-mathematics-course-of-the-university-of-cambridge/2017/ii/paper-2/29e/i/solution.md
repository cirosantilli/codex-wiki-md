<h1 id="29e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Keep $\nu$ fixed as $x\to+\infty$. On both vertical lines $\sin(\pm\pi+iy)=-i\sinh y$. The right side is traversed upward and the left downward, so their combined contribution is

$$
V(x)=-\frac{\sin(\pi\nu)}\pi\int_0^\infty e^{-x\sinh y-\nu y}\,dy.
$$

Set $v=\sinh y$. The [integral](../../../../../../integral.md) becomes $\int_0^\infty e^{-xv}a(v)\,dv$, where $a(v)=e^{-\nu\operatorname{arsinh}v}/\sqrt{1+v^2}$, $a(0)=1$ and $a'(0)=-\nu$. Successive [integration by parts](../../../../../../integration-by-parts.md), with exponentially vanishing terms at infinity, gives

$$
\int_0^\infty e^{-xv}a(v)\,dv=\frac1x-\frac\nu{x^2}+O(x^{-3}).
$$

Hence the leading vertical contribution is $\boxed{V(x)=-\sin(\pi\nu)/(\pi x)+O(x^{-2})}$. It is exactly zero for [integer](../../../../../../integer.md) $\nu$. These estimates hold for fixed real $\nu$; they are not uniform when the order grows with $x$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [29E](../../29e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="29a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Here $dy/ds=1$, $dx/ds=u^2$, $du/ds=0$, so from initial parameter $\xi$ we get $y=s$, $x=\xi+\xi^2y$ and $u=\xi$. Solving for the branch agreeing with $u=x$ at $y=0$, and rationalizing the apparent division by $y$, gives

$$
\boxed{u(x,y)=\frac{2x}{1+\sqrt{1+4xy}},\qquad1+4xy>0.}
$$

This formula is smooth on that [open set](../../../../../../open-set.md), which contains every point of the initial line. It satisfies $x=u+yu^2$ and $1+2yu=\sqrt{1+4xy}>0$. [Differentiation](../../../../../../differentiation.md) gives $u_x=1/(1+2yu)$, $u_y=-u^2/(1+2yu)$, verifying the equation and the data.

The transport field is $(u^2,1)$, with normal component one on $y=0$, so the initial line is everywhere non-characteristic. This explains why neighborhoods cover the entire initial line, although a single fixed-width strip need not work for unbounded $x$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [29A](../../29a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

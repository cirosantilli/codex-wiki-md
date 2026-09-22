<h1 id="b/5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The given stencil has nonnegative neighbor weights, zero row sums and a path from every unknown node to the Dirichlet boundary. Thus the [discrete maximum principle](../../../../../discrete-maximum-principle.md) applies, including at the reflected Neumann edge. The barrier is positive throughout the square.

At an ordinary interior node, central differences differentiate this quadratic exactly, giving $L_h\phi=2+2=4$. At $x=1$, the reflected horizontal part is

$$
\frac{2[\phi(1-h,y)-\phi(1,y)]}{h^2}=\frac4h+2,
$$

and the vertical part is two. Thus $L_h\phi=4+4/h$ there. Part (c) therefore permits

$$
C=\max\left\{\frac{K_1h^2}4,\frac{K_2h}{4+4/h}\right\}
=\frac{h^2}4\max\left\{K_1,\frac{K_2}{1+h}\right\}
\leq\frac{h^2}4\max\{K_1,K_2\}.
$$

On the Dirichlet boundary, the largest barrier value is $4+1/4=17/4$. Consequently

$$
\boxed{E\leq\frac{17}{16}\max\{K_1,K_2\}h^2,\qquad K_3=\frac{17}{16}\max\{K_1,K_2\}.}
$$

The $O(h)$ [truncation error](../../../../../truncation-error.md) at the Neumann edge is divided by the barrier response $O(h^{-1})$, producing a contribution of order $h^2$. Thus its lower local order does not reduce this global maximum-[norm](../../../../../norm.md) error bound.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the numerical solution of differential equations course of the University of Oxford](../../../../split.md)
6. [Numerical solution of differential equations course of the University of Oxford](../../../../../numerical-solution-of-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

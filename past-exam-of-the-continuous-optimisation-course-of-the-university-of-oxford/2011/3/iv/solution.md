<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Reverse the order of the two optimizations to obtain the [Lagrangian dual](../../../../lagrangian-duality.md)

$$
\sup_{y\in\mathbb R^m,\,\gamma\geq0}\ \inf_x\mathcal L(x,y,\gamma).
$$

Put $s=c-A^Ty$ and $r=\sqrt{s^TQ^{-1}s}$. For $\gamma>0$, completing the square gives

$$
x_{\min}=-\frac1{2\gamma}Q^{-1}s,\qquad
q(y,\gamma)=b^Ty-\gamma-\frac{r^2}{4\gamma}.
$$

At $\gamma=0$ the infimum is finite precisely if $s=0$, when it equals $b^Ty$. For $r>0$, the expression $\gamma+r^2/(4\gamma)$ is minimized at $\gamma=r/2$, with value $r$. The same optimized value holds when $r=0$, choosing $\gamma=0$. Eliminating $\gamma$ therefore gives $\sup_y\{b^Ty-\sqrt{s^TQ^{-1}s}\}$. Introducing $\theta=r$ yields

$$
\boxed{\max\{-\theta+b^Ty:A^Ty+s=c,\ s^TQ^{-1}s=\theta^2,\ \theta\geq0\}.}
$$

The nonnegative square root is enforced by $\theta\geq0$. Optimizers correspond by $\gamma=\theta/2$, including the zero case.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the continuous optimisation course of the University of Oxford](../../../split.md)
5. [Continuous optimisation course of the University of Oxford](../../../../continuous-optimisation-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

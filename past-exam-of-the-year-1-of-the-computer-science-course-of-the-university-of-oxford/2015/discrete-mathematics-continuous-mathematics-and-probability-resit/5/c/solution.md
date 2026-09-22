<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $g_1=x^2+y^2+z^2-4$ and $g_2=(x-3)^2+y^2+z^2-4$. Subtracting the two constraint equations gives $-6x+9=0$, hence $x=3/2$ and $y^2+z^2=7/4$. The feasible [set](../../../../../set-split.md) is therefore a [circle](../../../../../circle.md).

For [Lagrange multipliers](../../../../../lagrange-multiplier.md) $\lambda,\mu$, the stationarity equation $\nabla f=\lambda\nabla g_1+\mu\nabla g_2$ becomes

$$
0=2\lambda x+2\mu(x-3),\qquad
1=2(\lambda+\mu)y,\qquad
0=2(\lambda+\mu)z.
$$

At $x=3/2$, the first equation gives $\lambda=\mu$. The second ensures $\lambda+\mu\ne0$ and $y\ne0$, so the third gives $z=0$. The constraints then force $y=\pm\sqrt7/2$. Both points do satisfy the multiplier equations, taking $\lambda=\mu=1/(4y)$.

There are no missing singular constraint points: on the feasible [circle](../../../../../circle.md), the two constraint [gradients](../../../../../gradient.md) $(3,2y,2z)$ and $(-3,2y,2z)$ are [linearly independent](../../../../../linear-independence.md), since $y^2+z^2=7/4>0$. Thus the complete list of constrained [critical points](../../../../../critical-point.md) and [critical values](../../../../../critical-value.md) is

$$
\boxed{(x,y,z)=\left(\frac32,\pm\frac{\sqrt7}{2},0\right),\qquad f=\pm\frac{\sqrt7}{2}.}
$$

The bound $|y|\leq\sqrt7/2$ on the feasible [circle](../../../../../circle.md) shows that the positive value is the global [maximum](../../../../../maximum-of-a-subset-of-a-total-order.md) and the negative value is the global [minimum](../../../../../minimum-of-a-subset-of-a-total-order.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [Discrete mathematics, continuous mathematics, and probability (resit)](../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

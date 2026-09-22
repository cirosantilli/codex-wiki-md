<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Define $a_y=\min\{1,\lambda^y/7\}$. Given $Y=y$, the direct-return branch has [probability](../../../../../probability.md) $a_y$, while the fallback branch distributes its remaining mass uniformly over $0,\ldots,y$. The [law of total probability](../../../../../law-of-total-probability.md) therefore gives, for integer $x\geq0$,

$$
\boxed{\mathbb P(X=x)
=e^{-\lambda}\frac{\lambda^x}{x!}\min\!\left\{1,\frac{\lambda^x}{7}\right\}
+e^{-\lambda}\sum_{y=x}^{\infty}\frac{\lambda^y}{y!(y+1)}
\left(1-\min\!\left\{1,\frac{\lambda^y}{7}\right\}\right).}
$$

The summation includes $y=x$: a failed direct-return test can still return $x$ through the [discrete uniform distribution](../../../../../discrete-uniform-distribution.md) draw. There is no rejection loop and no additional normalization. Summing the displayed [probability mass function](../../../../../probability-mass-function.md) over $x$ gives $\sum_yp_y[a_y+(1-a_y)(y+1)/(y+1)]=1$. At $\lambda=1$, for example, $a_y=1/7$ at every $y$; it does not become one. This is an instance of the [accept-or-fallback mixture identity](../../../../../accept-or-fallback-mixture-identity.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the simulation and statistical programming course of the University of Oxford](../../../../split.md)
6. [Simulation and statistical programming course of the University of Oxford](../../../../../simulation-and-statistical-programming-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

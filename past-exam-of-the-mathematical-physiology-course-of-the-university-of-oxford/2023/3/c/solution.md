<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At any [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md), the first balance gives $u=\mu$ and the second gives $f(\mu,v)=0$. For every fixed $u>0$,

$$
f(u,0)=\frac{u^2}{1+u^2}>0,\qquad
\lim_{v\to\infty}f(u,v)=-\infty,
$$

and

$$
\boxed{f_v(u,v)=-\frac{u^4}{1+u^4}\frac{2v}{(1+v^2)^2}-\delta<0
\quad(v\ge0).}
$$

The [intermediate value theorem](../../../../intermediate-value-theorem.md) and strict [monotonicity](../../../../monotonic-function.md) give precisely one positive root $v=g(u)$ for each $u>0$. Since $f_v\ne0$, the [implicit function theorem](../../../../implicit-function-theorem.md) makes this a smooth [nullcline](../../../../nullcline.md). For every $\mu>0$, therefore,

$$
\boxed{(u_*,v_*)=(\mu,g(\mu))}
$$

is the unique positive [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md). Graphically, draw the vertical line $u=\mu$ through the given graph: it meets the graph once, even on its steep descending section. This vertical line is the condition for simultaneous stationarity; the full $u$ [nullcline](../../../../nullcline.md) at finite $\varepsilon$ is actually $f(u,v)=(\varepsilon/\gamma)(\mu-u)$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the mathematical physiology course of the University of Oxford](../../../split.md)
5. [Mathematical physiology course of the University of Oxford](../../../../mathematical-physiology-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

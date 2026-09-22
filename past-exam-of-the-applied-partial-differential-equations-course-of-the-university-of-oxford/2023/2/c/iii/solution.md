<h1 id="2/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $s_k(t)$ be the shock separating the fans from $k-1/2$ and $k+1/2$. Their traces give

$$
\dot s_k=\frac12\left[\frac{s_k-k+1/2}{t}+\frac{s_k-k-1/2}{t}\right]=\frac{s_k-k}{t},\qquad s_k(1)=k+1/2.
$$

Thus $\boxed{s_k(t)=k+t/2}$. Between consecutive shocks, $u=(x-k+1/2)/t$. Writing $\{r\}=r-\lfloor r\rfloor$ for the [fractional part](../../../../../fractional-part.md), the period-one solution can be expressed, with right-hand shock traces, as

$$
\boxed{u(x,t)=\frac12+\frac{\{x-t/2\}-1/2}{t},\qquad t\geq1}.
$$

To put it in the requested fixed-support sum, take

$$
\boxed{v(x,t)=\begin{cases}\displaystyle\frac12+\frac{\{x-t/2\}-1/2}{t},&-1/2\leq x<1/2,\\0,&\text{otherwise},\end{cases}\qquad u(x,t)=\sum_{k\in\mathbb Z}v(x-k,t)}.
$$

The half-open cells partition the line, so exactly one summand contributes at each point. This is a representation of the periodic solution, not a superposition principle for arbitrary solutions of a nonlinear equation.

The left and right shock states are $1/2+1/(2t)$ and $1/2-1/(2t)$; both average to the shock speed $1/2$, and the strict inequalities certify causality. The [periodic square-wave relaxation for the inviscid Burgers equation](../../../../../periodic-square-wave-relaxation-for-the-inviscid-burgers-equation.md) has the uniform estimate

$$
\boxed{\sup_x|u(x,t)-1/2|\leq\frac1{2t}\longrightarrow0}.
$$

The limit is the conserved mean $1/2$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the applied partial differential equations course of the University of Oxford](../../../../split.md)
6. [Applied partial differential equations course of the University of Oxford](../../../../../applied-partial-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

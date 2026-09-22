<h1 id="20/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For real square-integrable $f,g$, nonnegativity of $\int(f-\lambda g)^2dx$ gives a quadratic in the real number $\lambda$. If $\int g^2dx>0$, choose $\lambda=\int fg\,dx/\int g^2dx$ to obtain

$$
\left(\int fg\,dx\right)^2\leq\left(\int f^2dx\right)\left(\int g^2dx\right).
$$

If $\int g^2dx=0$, then $g=0$ almost everywhere and the same inequality is immediate. This proves the integral [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md).

Put $T=t_f-t_i>0$ and $L=x_f-x_i>0$. The forward [speed](../../../../../speed.md) satisfies $L=\int_{t_i}^{t_f}v\,dt$, so $V_t=L/T$. The [change of variables](../../../../../change-of-variables-formula.md) $dx=v\,dt$ gives $V_x=L^{-1}\int_{t_i}^{t_f}v^2dt$. Apply the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) to $v$ and the constant function one:

$$
L^2\leq T\int_{t_i}^{t_f}v^2dt,
\qquad\boxed{V_x\geq V_t.}
$$

Equality holds exactly when $v$ is constant almost everywhere. Equivalently, the [time and distance averages of speed](../../../../../time-and-distance-averages-of-speed.md) satisfy $V_x-V_t=\operatorname{Var}_t(v)/V_t$, which identifies the excess as a measure of speed variation.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [20](../../20.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

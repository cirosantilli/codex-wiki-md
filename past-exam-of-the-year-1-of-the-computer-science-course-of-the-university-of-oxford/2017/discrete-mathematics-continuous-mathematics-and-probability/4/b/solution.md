<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $\dot x=dx/du$, $\ddot x=d^2x/du^2$, $A_v=dA/dv$, $A_{vv}=d^2A/dv^2$, and $y_w=dy/dw$, $y_{ww}=d^2y/dw^2$. Put $S=A+A^T$. The [product rule](../../../../../product-rule.md) and [chain rule](../../../../../chain-rule.md) give

$$
\boxed{\begin{aligned}
f_u&=\dot x^TSx,\\
f_v&=x^TA_vx+w' y_w^Tb,\\
f_{uu}&=\ddot x^TSx+\dot x^TS\dot x,\\
f_{uv}&=\dot x^T(A_v+A_v^T)x,\\
f_{vv}&=x^TA_{vv}x+\bigl((w')^2y_{ww}+w''y_w\bigr)^Tb.
\end{aligned}}
$$

Here $w',w''$ are derivatives with respect to $v$. In the first derivative, $x^TA\dot x=\dot x^TA^Tx$ because the expression is scalar. Likewise $\dot x^TS\dot x=2\dot x^TA\dot x$ if desired. This [differentiation of a parameter-dependent quadratic form](../../../../../differentiation-of-a-parameter-dependent-quadratic-form.md) does not assume that $A$ is symmetric. The positive linear term $y^Tb$ contributes the positive chain-rule terms in the $v$ derivatives; it is independent of $u$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [Discrete mathematics, continuous mathematics and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

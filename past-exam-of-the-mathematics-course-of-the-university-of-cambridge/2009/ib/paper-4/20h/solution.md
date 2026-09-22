<h1 id="20h/solution">Solution</h1>

↑ **Parent:** [20H](../20h.md)

Interpret a beneficial trade as weakly improving both participants and strictly improving at least one; otherwise the identity trade would always remain available. Put $g_j=\nabla U_j(y_j)$. For a globally [strictly increasing concave function](../../../../../strictly-increasing-concave-function.md), every component of its gradient is strictly positive: [concavity](../../../../../concave-function.md) makes a coordinate derivative nonincreasing along that coordinate, and monotonicity makes it nonnegative. If it vanished at a finite point, it would vanish farther along the coordinate, contradicting strict increase on the whole real line.

To construct a [pairwise improvement from nonparallel utility gradients](../../../../../pairwise-improvement-from-nonparallel-utility-gradients.md), suppose two positive gradients $g,h$ are not proportional. Strict [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives

$$
\frac{g\cdot h}{\|h\|^2}<\frac{\|g\|^2}{g\cdot h}.
$$

Choose $t$ between these bounds and put $\delta=g-th$. Then $g\cdot\delta>0$ and $h\cdot\delta<0$. For sufficiently small $\varepsilon>0$, the feasible transfer $y_i\mapsto y_i+\varepsilon\delta$, $y_j\mapsto y_j-\varepsilon\delta$ strictly improves both utilities by [differentiability](../../../../../differentiability.md). This contradicts the absence of beneficial pairwise trades.

Hence all gradients are proportional. Choose $v=g_1$; positivity makes each proportionality scalar positive:

$$
\boxed{\nabla U_j(y_j)=\lambda_jv,\qquad\lambda_j>0.}
$$

Now take $\boxed{a_j=1/\lambda_j}$. The [concave supporting-tangent inequality](../../../../../concave-supporting-tangent-inequality.md) gives, for any other allocation $(z_j)$ with the same total endowment,

$$
\begin{aligned}
\sum_ja_jU_j(z_j)
&\leq\sum_ja_jU_j(y_j)+\sum_ja_j\nabla U_j(y_j)\cdot(z_j-y_j)\\
&=\sum_ja_jU_j(y_j)+v\cdot\sum_j(z_j-y_j)
=\sum_ja_jU_j(y_j).
\end{aligned}
$$

Thus the final allocations globally maximize the social planner's weighted objective. They need not be unique when utilities are not strictly concave, but the required positive supporting weights exist.

## ↑ Ancestors (10)

1. [20H](../20h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

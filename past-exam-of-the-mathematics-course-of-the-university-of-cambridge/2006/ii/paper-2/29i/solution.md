<h1 id="29i/solution">Solution</h1>

↑ **Parent:** [29I](../29i.md)

Let $V(x)=F(\pi,x)$ satisfy the Bellman optimality equation $V(x)=\sup_u\{r(x,u)+\beta E[V(x_1)\mid x,u]\}$. It is nonnegative because the rewards are. Under any competing policy, iterate its Bellman inequality to obtain $V(x)\ge E[\sum_{t=0}^{N-1}\beta^tr(x_t,u_t)+\beta^NV(x_N)]$. Drop the nonnegative terminal term and let $N\to\infty$. [Monotone convergence](../../../../../monotone-convergence-theorem.md) gives $V(x)\ge F(\widetilde\pi,x)$ for every competitor. Since $V$ is the actual return of $\pi$, this proves optimality without a transversality assumption.

Assume the income process remains nonnegative, as required by the feasible-control interval; for unrestricted feasible controls a sufficient condition is $\epsilon_t\ge-1$. If $\beta\le1/(1+\theta)<1$, spending everything gives constant income $x$ and value $V(x)=x/(1-\beta)$. Its Bellman expression for general $u$ is

$$
u+\frac{\beta}{1-\beta}\{x+\theta(x-u)\}=\frac{\beta(1+\theta)x+[1-\beta(1+\theta)]u}{1-\beta}.
$$

The coefficient of $u$ is nonnegative, so the maximum over $[0,x]$ occurs at $u=x$ and equals $V(x)$. Therefore **spending all income at every step is optimal**.

If $1/(1+\theta)<\beta<1$ and $x>0$, invest all income for $T$ steps and thereafter spend everything. Its expected return is $x[\beta(1+\theta)]^T/(1-\beta)$, unbounded as $T\to\infty$. In fact a sufficiently small fixed positive consumption fraction gives infinite expected discounted reward if $\beta[1+\theta(1-c)]\ge1$. Thus the value is infinite and the problem has no finite-valued optimum. For $\beta=1$, spending everything already gives infinite value when $x>0$. If $x=0$, the value is zero. A mean condition alone, without nonnegative income or equivalent admissibility restrictions, would not make the model well-defined.

## ↑ Ancestors (10)

1. [29I](../29i.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

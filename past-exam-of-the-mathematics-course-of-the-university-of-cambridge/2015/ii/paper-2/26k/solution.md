<h1 id="26k/solution">Solution</h1>

↑ **Parent:** [26K](../26k.md)

Write $V(x)=F(\pi,x)$. The [Bellman equation](../../../../../bellman-equation.md) implies $V(x)\geq r(x,u)+\beta\mathbb E[V(x_1)\mid x,u]$ for every available action. Under any competing policy, repeated conditioning gives

$$
V(x)\geq\mathbb E_{\pi'}\left[\sum_{t=0}^{n-1}\beta^tr(x_t,u_t)+\beta^nV(x_n)\right]\geq\mathbb E_{\pi'}\sum_{t=0}^{n-1}\beta^tr(x_t,u_t).
$$

The last inequality uses $V\geq0$. The [monotone convergence theorem](../../../../../monotone-convergence-theorem.md) now gives **$V(x)\geq F(\pi',x)$**, even when $\beta\geq1$. If $V(x)=\infty$ the comparison is immediate; otherwise the nonnegative conditional bounds justify each finite induction step. This proves [Bellman comparison with nonnegative rewards and superunit discount](../../../../../bellman-comparison-with-nonnegative-rewards-and-superunit-discount.md) without a vanishing-terminal-term assumption.

For the unit-bet policy in this [gambler's ruin](../../../../../gambler-s-ruin.md) problem, put $\beta=\sqrt{9/8}=3/(2\sqrt2)$. The value satisfies

$$
V_x=\beta\left(\frac13V_{x+1}+\frac23V_{x-1}\right),\qquad V_0=0,\quad V_{100}=100.
$$

The characteristic equation has the repeated root $\sqrt2$, so $V_x=(A+Bx)2^{x/2}$. The boundary values give

$$
\boxed{V_x=x\,2^{(x-100)/2}.}
$$

To justify that this finite recurrence solution is the expected reward despite $\beta>1$, let $Q$ be the transition matrix on transient states $1,\ldots,99$. The matrix $\beta Q$ is diagonally similar, with diagonal factors $2^{x/2}$, to the symmetric tridiagonal matrix with off-diagonal entries $1/2$. Its [eigenvalues](../../../../../eigenvalue.md) are $\cos(j\pi/100)$, $1\leq j\leq99$, with absolute value below one. Thus its [Neumann series](../../../../../neumann-series.md) converges and yields exactly the absorbed-payoff expectation and the unique recurrence solution.

When $p_2=1/4$, at wealth $2$ bet $2$ once and then follow the unit-bet policy. Its expected value is $\beta V_4/4=\beta V_2>V_2$, since $V_4=4V_2$. Therefore **the unit-bet policy is not optimal**.

## ↑ Ancestors (10)

1. [26K](../26k.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

<h1 id="30k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let the [value function](../../../../../../value-function.md) at time $n$ be the greatest conditional expected terminal utility attainable from wealth $x$. Independence of the innovations gives the [Bellman equation](../../../../../../bellman-equation.md)

$$
\boxed{
V(N,x)=U(x),\qquad
V(n,x)=\sup_{\theta\in\mathbb R^d}
\mathbb E\left[V\left(n+1,(1+r)x+\theta^T\xi_{n+1}\right)\right]
}
$$

for $0\leq n<N$. A policy obtained from the maximizing choices is admissible because each time-$n$ holding is a [predictable process](../../../../../../predictable-process.md), hence is known before $\xi_n$ is observed.

We prove the claimed properties by [backward induction](../../../../../../backward-induction.md). They hold at $n=N$ because $V(N,\cdot)=U$ is increasing and concave. Suppose they hold at time $n+1$. For fixed $\theta$, the map

$$
x\longmapsto
\mathbb E\left[V\left(n+1,(1+r)x+\theta^T\xi_{n+1}\right)\right]
$$

is increasing because $1+r>0$, and taking a supremum preserves this inequality.

For concavity, let $\theta_x$ and $\theta_y$ be optimal at wealths $x$ and $y$. For $0\leq t\leq1$, use the admissible portfolio

$$
\theta_t=t\theta_x+(1-t)\theta_y.
$$

The next wealth is the same [convex combination](../../../../../../convex-combination.md) of the next wealths generated from $(x,\theta_x)$ and $(y,\theta_y)$. Therefore

$$
\begin{aligned}
V(n,tx+(1-t)y)
&\geq\mathbb E\left[V\left(n+1,(1+r)(tx+(1-t)y)+\theta_t^T\xi_{n+1}\right)\right]\\
&\geq tV(n,x)+(1-t)V(n,y).
\end{aligned}
$$

This completes the induction and proves [monotonicity and concavity of a portfolio value function](../../../../../../monotonicity-and-concavity-of-a-portfolio-value-function.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [30K](../../30k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

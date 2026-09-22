<h1 id="23k/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

In an interval of length $t$, condition on the [Poisson process](../../../../../../poisson-process.md) count $X_t=k$. Independently marking its points gives $Y_t\mid X_t=k\sim\operatorname{Bin}(k,p)$. The joint [probability generating function](../../../../../../probability-generating-function.md) of kept and discarded counts is

$$
\mathbb E[s^{Y_t}u^{X_t-Y_t}]=\mathbb E[(ps+(1-p)u)^{X_t}]=\exp\{\lambda t[p(s-1)+(1-p)(u-1)]\}.
$$

It factors into the generating functions of independent Poisson variables of means $\lambda pt$ and $\lambda(1-p)t$. The same calculation applies to any interval, and counts and marks in disjoint intervals are independent. Hence **$Y$ is a Poisson process of intensity $\boxed{\lambda p}$**, and **$Y_t$ and $X_t-Y_t$ are independent**. This is the [Poisson thinning theorem](../../../../../../poisson-thinning-theorem.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [23K](../../23k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

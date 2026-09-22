<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $T=\tau_b\wedge\tau_{-a}$ and $A=\{\tau_b<\tau_{-a}\}$. The [Brownian exit time](../../../../../../brownian-exit-time.md) $T$ is finite almost surely. Optional stopping of the bounded martingale $B_{t\wedge T}$ gives

$$
\mathbb P(A)=\frac{a}{a+b}.
$$

For $T_n=T\wedge n$, optional stopping of $B_t^2-t$ gives $\mathbb ET_n=\mathbb E[B_{T_n}^2]\leq\max(a^2,b^2)$. Letting $n\to\infty$ by monotone and bounded convergence proves $\mathbb ET=\mathbb E[B_T^2]=ab$.

The third derivative in part b at $\lambda=0$ is the cubic martingale $B_t^3-3tB_t$. Optional stopping at $T_n$ is valid because $T_n$ is bounded. Since $B_{T_n}$ is bounded and $T_n\to T$ in $L^1$, its stopped identity passes to the limit and gives

$$
\mathbb E[B_T^3]=3\mathbb E[TB_T].
$$

Put $x=\mathbb E[T\mathbf1_A]$ and $y=\mathbb E[T\mathbf1_{A^c}]$. Then $x+y=ab$, while

$$
b x-a y
=\frac13\left(b^3\frac a{a+b}-a^3\frac b{a+b}\right)
=\frac{ab(b-a)}3.
$$

Solving gives $x=ab(2a+b)/(3(a+b))$. Dividing by $\mathbb P(A)=a/(a+b)$ proves the [conditional Brownian interval-exit time](../../../../../../conditional-brownian-interval-exit-time.md) formula

$$
\boxed{\mathbb E[\tau_b\mid\tau_b<\tau_{-a}]
=\frac{b^2+2ab}{3}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="25k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A rate-$\lambda$ [Poisson process](../../../../../../poisson-process.md) has $N_0=0$, right-continuous paths with upward jumps of size one, stationary [independent](../../../../../../independent-random-variables.md) increments, and $N_t-N_s\sim\operatorname{Poisson}(\lambda(t-s))$ for $t\geq s$. Assume $\lambda>0$. Its successive waiting times are [independent](../../../../../../independent-random-variables.md) exponential variables of rate $\lambda$. For $0<t_1<\cdots<t_n<t$, the product of their densities and the [probability](../../../../../../probability.md) of no further jump before $t$ is

$$
\lambda^ne^{-\lambda t_1}e^{-\lambda(t_2-t_1)}\cdots e^{-\lambda(t_n-t_{n-1})}e^{-\lambda(t-t_n)}=\lambda^ne^{-\lambda t}.
$$

Divide by $\mathbb P(N_t=n)=e^{-\lambda t}(\lambda t)^n/n!$ to obtain the conditional joint density

$$
\boxed{\frac{n!}{t^n}\mathbf1_{\{0<t_1<\cdots<t_n<t\}}.}
$$

Boundary inequalities do not affect a density. Equivalently these are the ordered values of $n$ [independent](../../../../../../independent-random-variables.md) uniform points of $[0,t]$. For $n=0$, the conditional tuple is empty.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [25K](../../25k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

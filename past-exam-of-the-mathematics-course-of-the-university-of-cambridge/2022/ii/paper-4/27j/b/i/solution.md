<h1 id="27j/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

With state-dependent admission, the effective birth rate in state $n$ is

$$
b_n=\lambda p(n)=\frac{\lambda}{n+1},
$$

while the death rate is $\mu$ for $n\geq1$. The stationary ratios for an [M-M-1 queue with state-dependent admission](../../../../../../../m-m-1-queue-with-state-dependent-admission.md) are therefore

$$
\frac{\pi_{n+1}}{\pi_n}=\frac{\rho}{n+1}.
$$

Induction gives $\pi_n=\pi_0\rho^n/n!$, and normalization identifies a [Poisson distribution](../../../../../../../poisson-distribution.md) of mean $\rho$:

$$
\boxed{\pi_n=e^{-\rho}\frac{\rho^n}{n!}}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [27J](../../../27j.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

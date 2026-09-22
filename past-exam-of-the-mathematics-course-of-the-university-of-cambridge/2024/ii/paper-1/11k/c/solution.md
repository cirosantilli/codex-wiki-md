<h1 id="11k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[Shannon second coding theorem](../../../../../../noisy-channel-coding-theorem.md) states that the operational capacity of a discrete memoryless channel equals

$$
C=\max_{P_X}I(X;Y):
$$

every rate below $C$ is achievable with error probability tending to zero, while rates above $C$ are not.

Put $d=b-a$. If $d=0$, then $Y=X+a$, so $X$ is recovered exactly and $C=1$ bit. If $|d|\geq2$, the two output supports

$$
\{a,b\},\qquad\{a+1,b+1\}
$$

are disjoint, so again $Y$ determines $X$ and $C=1$.

If $|d|=1$, one output value is common to both inputs and occurs with probability $1/2$ independently of the input, while either of the other two values reveals the input. The channel is therefore a binary erasure channel with erasure probability $1/2$, whose capacity is $1/2$ bit. Hence

$$
\boxed{
C=\begin{cases}
1/2,&|b-a|=1,\\
1,&|b-a|\ne1.
\end{cases}}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [11K](../../11k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

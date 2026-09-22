<h1 id="27i/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The first arrival time $A$ has an [exponential distribution](../../../../../../exponential-distribution.md) of rate $\lambda$ and is independent of the following [busy period](../../../../../../busy-period.md). Thus

$$
\phi_{T_k}(\theta)=\frac{\lambda}{\lambda-\theta}\phi_{B_k}(\theta).
$$

Substitute $\phi_{B_k}=(\lambda-\theta)\phi_{T_k}/\lambda$ into part (c). Its service-transform argument becomes $\theta+\lambda(\phi_{B_k}-1)=(\lambda-\theta)(\phi_{T_k}-1)$. Therefore

$$
\boxed{\frac{\lambda-\theta}{\lambda}\phi_{T_k}(\theta)
=\phi_{S_k}((\lambda-\theta)(\phi_{T_k}(\theta)-1))}.
$$

As before, positive arguments must lie in the domain of finite moment-generating functions.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [27I](../../27i.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

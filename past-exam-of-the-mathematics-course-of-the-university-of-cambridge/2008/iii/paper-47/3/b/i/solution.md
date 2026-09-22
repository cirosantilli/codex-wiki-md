<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For rate $\lambda>0$, the [exponential distribution](../../../../../../../exponential-distribution.md) has [cumulative distribution function](../../../../../../../cumulative-distribution-function.md) $F(x)=1-e^{-\lambda x}$ on $x\geq0$. [Inverse transform sampling](../../../../../../../inverse-transform-sampling.md) gives $-\log(1-U)/\lambda$; since $1-U$ is also uniform, an equivalent answer is

$$
\boxed{E=-\log U/\lambda.}
$$

For $x\geq0$, $P(E>x)=P(U<e^{-\lambda x})=e^{-\lambda x}$, verifying the [exponential distribution](../../../../../../../exponential-distribution.md) directly.

The centered [Laplace distribution](../../../../../../../laplace-distribution.md) with density $(\lambda/2)e^{-\lambda|x|}$ can be obtained by multiplying $E$ by an independent sign taking $1$ and $-1$ with equal probabilities. Alternatively, its [inverse transform sampling](../../../../../../../inverse-transform-sampling.md) formula uses just one uniform variate:

$$
\boxed{L=\begin{cases}\log(2U)/\lambda,&0<U<1/2,\\-\log(2(1-U))/\lambda,&1/2\leq U<1.\end{cases}}
$$

The first branch inverts the negative half of the [cumulative distribution function](../../../../../../../cumulative-distribution-function.md) and the second branch inverts the positive half. Add a location parameter if a noncentered [Laplace distribution](../../../../../../../laplace-distribution.md) is wanted.

**Correct uniformity is essential for each marginal distribution, and independence is essential for independent samples and for the sign construction.** For example, setting every $U_i$ equal to a single uniform $U$ gives uniform marginals but identical transformed draws. Likewise, choosing a sign from the same uniform used for the magnitude can change the [Laplace distribution](../../../../../../../laplace-distribution.md) unless the one-uniform inverse above is used.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 47](../../../../paper-47-split.md)
5. [Iii](../../../../split.md)
6. [2008](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

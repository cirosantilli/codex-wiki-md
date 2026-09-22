# Sign and phase in power iteration

↑ **Parent:** [Power iteration](power-iteration.md)

Under [power iteration convergence for a diagonalizable matrix](power-iteration-convergence-for-a-diagonalizable-matrix.md), take $v_1=u_1$ to be a [unit vector](unit-vector.md). The displayed formula describes both the dominant [eigenvector](eigenvector.md) direction and its rotating complex unit factor. With real data and a positive [dominant eigenvalue](dominant-eigenvalue.md), $x_k$ converges to $u_1$ or $-u_1$ according to the sign of $c_1$. With a negative [dominant eigenvalue](dominant-eigenvalue.md), consecutive [vectors](vector.md) approach opposite signs even though their [power iteration direction error](power-iteration-direction-error.md) tends to zero.

For complex data write $\lambda_1=|\lambda_1|e^{i\phi}$, where $\phi$ is its [complex argument](argument-complex-analysis.md). The leading factor turns by $e^{i\phi}$ per step, so the [vectors](vector.md) generally do not converge. For example, $A=\operatorname{diag}(2i,1)$ and $x_0=(1,1)^T/\sqrt2$ give $A^kx_0=((2i)^k,1)^T/\sqrt2$: the first component cycles through four phases while the ratio of component [moduli](modulus.md) tends to zero. Its [power iteration direction error](power-iteration-direction-error.md) is $2^{-k}/\sqrt{1+2^{-2k}}$. Multiplying $x_k$ by $e^{-i(\arg c_1+k\phi)}$ gives a sequence converging to $u_1$.

A stopping rule based only on $\|x_{k+1}-x_k\|_2$ therefore rejects successful sign-alternating iterations. A comparison invariant under complex unit factors is

$$
\min_{|\omega|=1}\|x_{k+1}-\omega x_k\|_2=\sqrt{2-2|x_k^*x_{k+1}|}.
$$

Even this comparison can be small for a slowly changing wrong mixture; the [eigenpair residual](eigenpair-residual.md) supplies a separate diagnostic.

## ↑ Ancestors (7)

1. [Power iteration](power-iteration.md)
2. [Numerical linear algebra](numerical-linear-algebra-split.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Power iteration failure cases](power-iteration-failure-cases.md)

<h1 id="26j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Convolve three rate-$\lambda$ [exponential distributions](../../../../../../exponential-distribution.md). The first two have convolution density $\lambda^2xe^{-\lambda x}\mathbf1_{x>0}$; convolving once more gives

$$
\int_0^x\lambda^2s e^{-\lambda s}\lambda e^{-\lambda(x-s)}ds=\frac12\lambda^3x^2e^{-\lambda x}.
$$

Thus $X$ is an [Erlang distribution](../../../../../../erlang-distribution.md) of shape three, equal in law to the sum of three independent exponentials. Addition of independent means and variances yields

$$
\boxed{\mathbb EX=3/\lambda,\quad\operatorname{Var}X=3/\lambda^2,\quad M_X(t)=\left(\frac\lambda{\lambda-t}\right)^3\ (t<\lambda).}
$$

For $t\ge\lambda$ the [moment-generating function](../../../../../../moment-generating-function.md) is infinite.

Realize each [holding time](../../../../../../holding-time.md) as a consecutive block of three exponential holding times from one [Poisson process](../../../../../../poisson-process.md) $N_t$. The renewal count is then $X_t=\lfloor N_t/3\rfloor$ pathwise under this coupling. If $R_t$ is the remainder of $N_t$ modulo three, $N_t=3X_t+R_t$ and $\mathbb ER_t=p_1(t)+2p_2(t)$. Taking expectations gives

$$
\boxed{m(t)=\frac{\lambda t}{3}-\frac13p_1(t)-\frac23p_2(t).}
$$

This proves the formula without assuming that the renewal count itself is Poisson.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [26J](../../26j.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

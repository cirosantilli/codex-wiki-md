<h1 id="27l/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [size-biased distribution](../../../../../../size-biased-distribution.md) associated with $\xi_1$ is defined by

$$
\mathbb E h(\widehat\xi_1)
=\frac{\mathbb E[\xi_1h(\xi_1)]}{\mathbb E\xi_1}
=\lambda\mathbb E[\xi_1h(\xi_1)]
$$

for every bounded measurable $h$. Thus, if $\xi_1$ has density $f$, then $\widehat\xi_1$ has density $\lambda x f(x)$.

Now suppose that $\xi_1$ is exponential with rate $\lambda$. The renewal epochs form a [Poisson process](../../../../../../poisson-process.md). Write

$$
A_t=t-S_{N_t},\qquad R_t=S_{N_t+1}-t,
$$

so that $L(t)=A_t+R_t$. Independent stationary increments and the exponential waiting-time law show that $R_t$ is exponential with rate $\lambda$, independent of the history up to $t$ and hence of $A_t$. For fixed $a\geq0$ and $t>a$,

$$
\mathbb P(A_t>a)
=\mathbb P(N_t-N_{t-a}=0)
=e^{-\lambda a}.
$$

Consequently $A_t$ converges in distribution to another rate-$\lambda$ exponential variable, independent of $R_t$. Therefore $L(t)$ converges to the sum of two independent rate-$\lambda$ exponentials, whose density is

$$
\int_0^x\lambda e^{-\lambda y}\lambda e^{-\lambda(x-y)}\,dy
=\lambda^2xe^{-\lambda x}.
$$

The size-biased density of $\xi_1$ is likewise

$$
\lambda x\big(\lambda e^{-\lambda x}\big)
=\lambda^2xe^{-\lambda x}.
$$

Hence the [exponential renewal interval limit](../../../../../../exponential-renewal-interval-limit.md) is

$$
\boxed{L(t)\xrightarrow{d}\widehat\xi_1}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [27L](../../27l.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

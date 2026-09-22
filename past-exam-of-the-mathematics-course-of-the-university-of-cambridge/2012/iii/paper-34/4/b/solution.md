<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

One continuous [Girsanov theorem](../../../../../../girsanov-theorem.md) formulation is as follows. Let $L$ be a zero-starting continuous local [martingale](../../../../../../martingale-split.md) such that $Z=\mathcal E(L)$ is a strictly positive [uniformly integrable](../../../../../../uniform-integrability.md) [martingale](../../../../../../martingale-split.md), and define $d\mathbb Q=Z_\infty\,d\mathbb P$. For every continuous $\mathbb P$-local [martingale](../../../../../../martingale-split.md) $N$,

$$
\boxed{N-[N,L]\text{ is a }\mathbb Q\text{-local martingale}.}
$$

On a finite horizon the same assertion holds with terminal density $Z_T$, provided $Z$ is a true [martingale](../../../../../../martingale-split.md) through $T$. In particular, if $L_t=\int_0^t\theta_s\,dB_s$, then

$$
\widetilde B_t=B_t-\int_0^t\theta_s\,ds
$$

is a [Brownian motion](../../../../../../brownian-motion-split.md) under $\mathbb Q$, on the specified horizon. Its [quadratic variation](../../../../../../quadratic-variation.md) remains $t$ under this absolutely continuous measure (equivalent on every finite-horizon sigma-algebra), and the [Lévy characterization of Brownian motion](../../../../../../levy-characterization-of-brownian-motion.md) identifies it as Brownian. The density sign and drift subtraction are paired: choosing the exponential of $-\int\theta\,dB$ instead produces $B+\int\theta\,ds$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

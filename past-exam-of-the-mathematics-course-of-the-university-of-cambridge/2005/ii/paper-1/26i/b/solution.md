<h1 id="26i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

With two offspring always, the backward equation becomes $\phi'=\mu(\phi^2-\phi)$. Separation and the initial value give

$$
\phi_t(s)=\frac{se^{-\mu t}}{1-s(1-e^{-\mu t})}=\sum_{k\ge1}e^{-\mu t}(1-e^{-\mu t})^{k-1}s^k.
$$

Thus $M_t$ is geometric on the positive integers, and

$$
\boxed{P(N_t=j)=e^{-\mu t}(1-e^{-\mu t})^j,\qquad j=0,1,\ldots.}
$$

This is a [Yule process](../../../../../../yule-process.md) shifted down by one. It is **not an inhomogeneous [Poisson process](../../../../../../poisson-process.md)**. Given $N_t=j$, its instantaneous jump rate is $\mu(j+1)$, a state-dependent random rate rather than a deterministic function of time. Also $E[N_t]=e^{\mu t}-1$ whereas $\operatorname{Var}(N_t)=e^{\mu t}(e^{\mu t}-1)$, unequal to the mean for $t>0$. Its mean arrival intensity $\mu e^{\mu t}$ does not turn its dependent increments and geometric marginals into Poisson ones.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [26I](../../26i.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

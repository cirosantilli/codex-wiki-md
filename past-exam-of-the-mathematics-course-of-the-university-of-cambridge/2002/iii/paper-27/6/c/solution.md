<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For each fixed $m\ge0$ and $T\ge m$, remove the first $m$ weight factors but retain the same walk law:

$$
Z_T^{(m)}=\left\langle\prod_{j=m+1}^T(1+\varepsilon h(j,\xi_j))\right\rangle.
$$

This quantity is measurable with respect to $\mathcal G_{m+1}=\sigma(h(j,x):j\ge m+1,x\in\mathbb Z^d)$, since the averaging over all walk positions is deterministic and involves no earlier environment variables. The bounds on each deleted factor give, pointwise for every environment,

$$
(1-\varepsilon)^mZ_T^{(m)}\le Z_T\le(1+\varepsilon)^mZ_T^{(m)}.
$$

Both constants are finite and strictly positive. Taking lower limits gives the exact identity of events

$$
\{\liminf_TZ_T=0\}=\{\liminf_TZ_T^{(m)}=0\}\in\mathcal G_{m+1}.
$$

There is no exceptional-set issue in this comparison. Choose the version of $\zeta$ to equal $\liminf_TZ_T$ when this is finite and to equal $1$ otherwise; it agrees with the almost-sure [martingale](../../../../../../martingale-split.md) limit, and its zero event is precisely the left-hand event above. Since the identity holds for every $m$, $\{\zeta=0\}$ belongs to the printed [tail sigma-algebra](../../../../../../tail-sigma-algebra.md) $\bigcap_{n\ge1}\mathcal G_n$. This proves the [tail event for a vanishing positive path-weight limit](../../../../../../tail-event-for-a-vanishing-positive-path-weight-limit.md) without pretending that the whole value of $\zeta$ is tail-measurable.

The [independent](../../../../../../independent-random-variables.md) time layers of the environment are [independent](../../../../../../independent-random-variables.md) random vectors, so the [Kolmogorov zero-one law](../../../../../../kolmogorov-s-zero-one-law.md) applies to their [tail sigma-algebra](../../../../../../tail-sigma-algebra.md). It yields $\mathbb P(\zeta=0)\in\{0,1\}$. Under the small-noise condition from part (b), $\mathbb E\zeta=1$ and $\zeta\ge0$, so that probability cannot be $1$. Hence

$$
\boxed{\mathbb P(\zeta=0)=0,\qquad \zeta>0\text{ almost surely}.}
$$

The tail-event argument itself works for every $0<\varepsilon<1$; the deduction of positivity here uses the mean-one conclusion supplied by part (b).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

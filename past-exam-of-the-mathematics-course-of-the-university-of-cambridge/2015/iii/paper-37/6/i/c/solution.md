<h1 id="6/i/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $k\in\mathcal N_i$, put $a_k^{(i)}=\sum_{j\in\mathcal N_k\setminus\{i\}}s_j$ and $H_i=\sum_{j\in\mathcal N_i}s_j$. Removing all factors independent of $s_i$ from the [posterior distribution](../../../../../../../bayesian-posterior.md) gives, for $u\in\{-1,1\}$,

$$
w_i(u)=\exp\!\left[-JuH_i-\frac12\sum_{k\in\mathcal N_i}\{x_k-(a_k^{(i)}+u)^7\}^2\right],\qquad
\boxed{\pi_i(u\mid s_{-i},x)=\frac{w_i(u)}{w_i(+1)+w_i(-1)}.}
$$

A stable implementation uses the difference of the log weights. The conditional [log odds](../../../../../../../log-odds.md) are

$$
L_i=-2JH_i-\frac12\sum_{k\in\mathcal N_i}
\left[\{x_k-(a_k^{(i)}+1)^7\}^2-\{x_k-(a_k^{(i)}-1)^7\}^2\right],
$$

so $\pi_i(+1\mid s_{-i},x)=1/(1+e^{-L_i})$, a [logistic function](../../../../../../../logistic-function.md). For very large $|L_i|$, evaluate this logistic expression using the sign of $L_i$ to avoid exponential overflow.

For [Gibbs sampling for a finite hidden spin field](../../../../../../../gibbs-sampling-for-a-finite-hidden-spin-field.md), initialize any spin configuration. At every step choose $i\in D$ uniformly, draw a fresh uniform variable, set spin $i$ to $+1$ with the probability above and to $-1$ otherwise, and leave all remaining spins fixed. This [Random-scan Gibbs sampler](../../../../../../../random-scan-gibbs-sampler.md) has the stated [posterior distribution](../../../../../../../bayesian-posterior.md) invariant by [detailed balance of a random-scan Gibbs sampler](../../../../../../../detailed-balance-of-a-random-scan-gibbs-sampler.md). All [conditional probabilities](../../../../../../../conditional-probability.md) are strictly between zero and one. For the one-site case, the [conditional probabilities](../../../../../../../conditional-probability.md) are both $1/2$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [I](../../i.md)
3. [6](../../../6.md)
4. [Paper 37](../../../../paper-37-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

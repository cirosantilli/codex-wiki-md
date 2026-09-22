<h1 id="26j/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

At a state with positive departure rate $\lambda_i=R-r_i$, the next-jump probabilities are

$$
\boxed{\widehat p_{ij}=\frac{r_j}{R-r_i}\ (j\ne i),\qquad\widehat p_{ii}=0.}
$$

If at least two rates are positive, every state has positive departure rate and the normalizing constant $Z=\sum_i r_i(R-r_i)=R^2-\sum_i r_i^2$ is positive. The jump-chain equilibrium law is

$$
\boxed{\widehat\pi_i=\frac{r_i(R-r_i)}{Z}.}
$$

Indeed $\widehat\pi_i\widehat p_{ij}=r_ir_j/Z$ is symmetric, proving both stationarity and reversibility. Jump observations weight the continuous-time equilibrium by the departure rate, so $\widehat\pi$ is generally different from $\pi$.

If exactly one rate, $r_k$, is positive, state $k$ is absorbing and the denominator $R-r_k$ vanishes. There is no next jump from that state: the genuine embedded jump sequence terminates there. Under the usual extended-chain convention set $\widehat p_{kk}=1$; every other state jumps to $k$ with [probability](../../../../../../probability.md) one. Its equilibrium law is $\delta_k$ and it is trivially reversible there. The normalized $r_i(R-r_i)$ formula cannot be used in that absorbing case.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [26J](../../26j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

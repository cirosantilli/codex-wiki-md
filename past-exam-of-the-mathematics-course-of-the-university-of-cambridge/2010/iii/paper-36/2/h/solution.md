<h1 id="2/h/solution">Solution</h1>

↑ **Parent:** [H](../h.md)

The [posterior probability](../../../../../../posterior-probability.md) $q_i=\mathbb P(\lambda_i>1\mid y_i)$ answers a natural directional question: how likely is this area's risk to exceed the reference risk? It accounts for uncertainty rather than declaring an increase from the point estimate alone. However, it does not distinguish a negligible increase from a clinically important one, and it combines prior beliefs with evidence from the data. With an informative [prior distribution](../../../../../../prior-probability.md), a large probability may already have been present before observation, or a genuinely surprising count may be strongly moderated by the prior.

To measure the evidence supplied by the observations, compare posterior and prior odds. If $q_0=\mathbb P(\lambda_i>1)$ under the chosen proper [prior distribution](../../../../../../prior-probability.md), the [Bayes factor](../../../../../../bayes-factor.md) for increased versus nonincreased risk is

$$
\boxed{B_{+,-}(y_i)=\frac{q_i/(1-q_i)}{q_0/(1-q_0)}.}
$$

This follows from the [posterior odds](../../../../../../posterior-odds.md) identity when the two models use the original prior conditioned respectively on $\lambda_i>1$ and $\lambda_i\le1$. For the specified prior, $q_0$ is the upper tail at one of $\operatorname{Gamma}(16,16)$; centering its mean at one does not make this tail probability exactly $1/2$. To address seriousness itself, choose a substantive excess $c>0$ and report **the posterior probability of $\lambda_i>1+c$**, together with an interval for the size of the excess. An evidence ratio and a meaningful risk threshold answer different, complementary questions.

## ↑ Ancestors (11)

1. [H](../h.md)
2. [2](../../2.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

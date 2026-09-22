<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $N=4700$ and let the daily distances be [independent and identically distributed random variables](../../../../../independent-and-identically-distributed-random-variables.md) with probabilities $p_1=p_3=0.4995$, $p_{100}=0.001$. The unconditioned mean daily distance is $2.098$, whereas the observed trip requires a daily average near $10$. Conditioning on that rare average changes the typical frequencies substantially. It does not determine an exact boost count.

Use the [method of types](../../../../../method-of-types.md): for a fixed finite alphabet, the probability of an [empirical distribution](../../../../../type-information-theory.md) $q$ is

$$
\mathbb P(\text{type }q)
=\frac{N!}{\prod_i(Nq_i)!}\prod_i p_i^{Nq_i}
=\exp[-ND(q\Vert p)+O(\log N)],
$$

where $D(q\Vert p)=\sum_iq_i\log(q_i/p_i)$ is [relative entropy](../../../../../kullback-leibler-divergence.md), using [natural logarithms](../../../../../natural-logarithm.md). This follows directly from [Stirling's approximation](../../../../../stirling-formula.md). There are only polynomially many types, so the [empirical distribution](../../../../../type-information-theory.md) conditional on a mean constraint concentrates at its unique [relative entropy](../../../../../kullback-leibler-divergence.md) minimizer, when admissible lattice types approximate that minimizer. Any fixed neighborhood of it has a strictly smaller minimum cost than its complement.

Minimize $D(q\Vert p)$ subject to $\sum_iq_i=1$ and $q_1+3q_3+100q_{100}=10$. The [entropy minimization under a prescribed sample mean](../../../../../entropy-minimization-under-a-prescribed-sample-mean.md) gives the [exponential tilting](../../../../../exponential-tilting.md)

$$
q_i=\frac{p_i e^{\theta i}}{Z(\theta)},\qquad
Z(\theta)=0.4995e^\theta+0.4995e^{3\theta}+0.001e^{100\theta}.
$$

To verify minimization without relying only on [Lagrange multipliers](../../../../../lagrange-multiplier.md), any feasible distribution $r$ satisfies

$$
D(r\Vert p)=D(r\Vert q)+10\theta-\log Z(\theta).
$$

[Relative entropy nonnegativity](../../../../../relative-entropy-nonnegativity.md) makes $q$ the unique minimizer. Its mean determines $\theta$ through $Z'(\theta)/Z(\theta)=10$, or

$$
0.09e^{100\theta}
=0.4995(9e^\theta+7e^{3\theta}).
$$

The derivative of the tilted mean is the tilted [variance](../../../../../variance-split.md), which is strictly positive. The mean rises from $2.098$ at $\theta=0$ to $100$ as $\theta\to\infty$, so this equation has one positive solution. Numerically,

$$
\theta=0.0457316645,\qquad
(q_1,q_3,q_{100})
=(0.4384035050,\ 0.4803922990,\ 0.0812041960).
$$

The predicted boost count is $Nq_{100}=381.6597211$. Thus **the conditional large-deviation estimate is about 382 boosts**.

For exact arrival at total distance $47000$, let $k,m,l$ count days of distances $100,3,1$. The constraints give

$$
k+m+l=4700,\qquad 99k+2m=42300.
$$

Consequently $k$ can be any even integer from $340$ to $426$. In particular, a unique count cannot be inferred from the return time. The exact conditional weights are proportional to

$$
\frac{4700!}{k!\,m!\,l!}(0.001)^k(0.4995)^{4700-k},
\qquad m=\frac{42300-99k}{2},\quad l=4700-k-m.
$$

Their most probable count is $k=382$, consistent with the [exponential tilting](../../../../../exponential-tilting.md) calculation. This finite-sample inference is a [conditional probability](../../../../../conditional-probability.md) statement, not an assertion that all journeys with the stated duration have that count.

If returning home means first crossing the distance threshold on day $4700$, the final total instead lies between $47000$ and $47099$. The last increment must exceed the overshoot; for fixed counts this selects the corresponding fraction of possible last days. Near the tilted optimum that factor is bounded away from zero, so it does not alter the leading exponential type cost. The same approximate answer follows. Exact conditional enumeration of this first-arrival interpretation also has mode $382$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 77](../../paper-77-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

<h1 id="1/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Choose versions

$$
p_k=\mathbb E[\mathbf1_{B_k}\mid\mathcal F_{k-1}]\in[0,1],\qquad A_0=0,\qquad A_n=\sum_{k=1}^np_k.
$$

The [stochastic process](../../../../../stochastic-process-split.md) $(A_n)$ is increasing, and its $k$th increment is $\mathcal F_{k-1}$-[measurable](../../../../../measurability.md), so it is [predictable](../../../../../predictable-process.md). The [Doob decomposition theorem](../../../../../doob-decomposition-theorem.md) therefore gives

$$
\boxed{X_n=M_n+A_n,\qquad M_0=0,\qquad M_n=\sum_{k=1}^n(\mathbf1_{B_k}-p_k).}
$$

To check the [martingale](../../../../../martingale-split.md) property directly, each summand is [integrable](../../../../../integrability.md) and has zero [conditional expectation](../../../../../conditional-expectation.md) given $\mathcal F_{k-1}$. The sums are an [adapted process](../../../../../adapted-process.md) for the given [filtration](../../../../../filtration-probability-theory.md). Thus $\mathbb E[M_n\mid\mathcal F_{n-1}]=M_{n-1}$. Its [bounded increments](../../../../../bounded-increments.md) satisfy $|M_n-M_{n-1}|\leq1$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [D](../../d.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the probability, measure and martingales course of the University of Oxford](../../../../split.md)
6. [Probability, measure and martingales course of the University of Oxford](../../../../../probability-measure-and-martingales-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

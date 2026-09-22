<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [floor function](../../../../../floor-function.md) gives the deterministic bound

$$
0\leq X-X_n<2^{-n}
$$

for every outcome, including $X=1$. Thus **all three convergence assertions hold**: there is pointwise, and hence [almost sure convergence](../../../../../almost-sure-convergence.md), as well as [convergence in probability](../../../../../convergence-in-probability.md) and [convergence in L2](../../../../../convergence-in-l2.md). In detail, for $\varepsilon>0$ the [probability](../../../../../probability.md) $\mathbb P(|X-X_n|>\varepsilon)$ is zero as soon as $2^{-n}\leq\varepsilon$; also

$$
\mathbb E[|X-X_n|^2]\leq4^{-n}\longrightarrow0.
$$

The [uniform distribution](../../../../../continuous-uniform-distribution.md) even gives the exact [second moment](../../../../../second-moment.md) of the error by integrating over the [dyadic partition](../../../../../dyadic-partition.md):

$$
\boxed{\mathbb E[|X-X_n|^2]=2^n\int_0^{2^{-n}}t^2\,dt=\frac{4^{-n}}3.}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
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

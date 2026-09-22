<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the nonnegative [martingale](../../../../../martingale-split.md) $(Y_n)$ and [filtration](../../../../../filtration-probability-theory.md) $(\mathcal H_n)$ established above. Fix a finite $n$ and let

$$
H=\{\max_{1\leq k\leq n}Y_k\geq\lambda\},\qquad
T=\min\bigl(\{1\leq k\leq n:Y_k\geq\lambda\}\cup\{n\}\bigr).
$$

For $j<n$, $\{T\leq j\}$ is the [union](../../../../../set-union.md) of the threshold-crossing [events](../../../../../event.md) up to $j$, so $T$ is a [bounded stopping time](../../../../../bounded-stopping-time.md). The [optional stopping theorem](../../../../../optional-sampling-theorem-for-a-supermartingale.md) for a [martingale](../../../../../martingale-split.md) at a [bounded stopping time](../../../../../bounded-stopping-time.md) gives $\mathbb EY_T=\mathbb EY_0=1$. On $H$ one has $Y_T\geq\lambda$; on its [complement](../../../../../complement-of-a-set.md) one still has $Y_T\geq0$. Therefore

$$
\lambda\mathbb P(H)\leq\mathbb EY_T=1,
\qquad
\boxed{\mathbb P(H)\leq\lambda^{-1}.}
$$

Only a [bounded stopping time](../../../../../bounded-stopping-time.md) has been used, so no extra [uniform integrability](../../../../../uniform-integrability.md) assumption at an unbounded hitting time is implicit. This is also the [Doob maximal inequality for a nonnegative submartingale](../../../../../doob-maximal-inequality-for-a-nonnegative-submartingale.md) specialized to a mean-one [martingale](../../../../../martingale-split.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the probability, measure and martingales course of the University of Oxford](../../../../split.md)
6. [Probability, measure and martingales course of the University of Oxford](../../../../../probability-measure-and-martingales-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

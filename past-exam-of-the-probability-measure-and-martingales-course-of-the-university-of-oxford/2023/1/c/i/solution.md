<h1 id="1/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The first entrance time $\tau_K$ is a [stopping time](../../../../../stopping-time.md), because $\{\tau_K\leq n\}=\bigcup_{j=0}^n\{M_j\leq-K\}\in\mathcal F_n$. Before this time $M_n>-K$; at entrance, the [bounded increments](../../../../../bounded-increments.md) give $M_{\tau_K}>-K-L$. Thus the [stopped martingale](../../../../../stopped-martingale.md)

$$
N_n=M_{n\wedge\tau_K}+K+L
$$

is a [nonnegative martingale](../../../../../nonnegative-martingale.md). Here the [stopped process](../../../../../stopped-process.md) is a [martingale](../../../../../martingale-split.md) since its increment is $\mathbf1_{\{\tau_K>n\}}(M_{n+1}-M_n)$, whose [conditional expectation](../../../../../conditional-expectation.md) given $\mathcal F_n$ is zero.

The [martingale convergence theorem](../../../../../martingale-convergence-theorem.md) states that a [nonnegative martingale](../../../../../nonnegative-martingale.md) converges [almost surely](../../../../../almost-sure-convergence.md) to a finite [integrable random variable](../../../../../integrable-random-variable.md); indeed its [expectations](../../../../../expected-value-split.md) are constant, giving the required bound in the [L1 norm](../../../../../l1-norm.md). Apply this theorem to $(N_n)$. On $\{\tau_K=\infty\}$ the [stopped process](../../../../../stopped-process.md) equals the original one at every time. Hence

$$
\boxed{M_n\text{ converges to a finite limit almost surely on }\{\tau_K=\infty\}.}
$$

The overshoot bound is why the assumption of [bounded increments](../../../../../bounded-increments.md) matters.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
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

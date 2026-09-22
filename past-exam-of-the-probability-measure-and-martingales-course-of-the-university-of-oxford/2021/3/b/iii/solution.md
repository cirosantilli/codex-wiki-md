<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [optional stopping theorem](../../../../../optional-sampling-theorem-for-a-supermartingale.md) at a [bounded stopping time](../../../../../bounded-stopping-time.md) states that an [integrable](../../../../../integrability.md) [martingale](../../../../../martingale-split.md) $Z_n$ satisfies $\mathbb EZ_T=\mathbb EZ_0$ whenever $T\leq n$ for a fixed finite $n$. Apply this first to $S$ at $T=n\wedge\tau$. The [simple symmetric random walk](../../../../../simple-symmetric-random-walk.md) cannot cross an integer endpoint without hitting it, so

$$
a\leq S_{n\wedge\tau}\leq b,\qquad
\mathbb E S_{n\wedge\tau}=0.
$$

The preceding part gives $\tau<\infty$ [almost surely](../../../../../almost-sure-convergence.md), hence $S_{n\wedge\tau}\to S_\tau$ [almost surely](../../../../../almost-sure-convergence.md). The constant bound $C=\max\{-a,b\}$ permits the [dominated convergence theorem](../../../../../dominated-convergence-theorem.md), yielding $\mathbb ES_\tau=0$. Since $S_\tau$ is either $a$ or $b$, solving $ap+b(1-p)=0$ gives its full [probability distribution](../../../../../probability-distribution-split.md):

$$
\boxed{\mathbb P(S_\tau=a)=\frac{b}{b-a},\qquad
\mathbb P(S_\tau=b)=\frac{-a}{b-a}.}
$$

Now let

$$
L_\tau=\sum_{k=0}^{\tau-1}\mathbf1_{\{S_k=0\}}.
$$

This counts the visit at time $0$, and excludes the exit time. Apply the same bounded-time [optional stopping theorem](../../../../../optional-sampling-theorem-for-a-supermartingale.md) to $M_n=|S_n|-L_n$. For each $n$ it gives

$$
\mathbb E L_{n\wedge\tau}=\mathbb E|S_{n\wedge\tau}|.
$$

The visit counts increase to $L_\tau$, so [monotone convergence](../../../../../monotone-convergence-theorem.md) applies to the left. [Dominated convergence](../../../../../dominated-convergence-theorem.md) applies to the right using $|S_{n\wedge\tau}|\leq C$. Consequently $L_\tau$ is an [integrable random variable](../../../../../integrable-random-variable.md) and

$$
\boxed{\mathbb E L_\tau=\mathbb E|S_\tau|
=(-a)\frac{b}{b-a}+b\frac{-a}{b-a}
=\frac{-2ab}{b-a}.}
$$

This is the origin case of [expected occupation before interval exit for a simple symmetric random walk](../../../../../expected-occupation-before-interval-exit-for-a-simple-symmetric-random-walk.md). The argument obtains [integrability](../../../../../integrability.md) of the total occupation count before using any unbounded-time [optional stopping](../../../../../optional-sampling-theorem-for-a-supermartingale.md) for $M$, so it does not presuppose the [uniform integrability](../../../../../uniform-integrability.md) asked about next. The endpoint [probabilities](../../../../../probability.md) also agree with the standard [gambler's ruin](../../../../../gambler-s-ruin.md) calculation.[§4.8.1, Theorem 4.8.7(a), printed pp. 257–258: symmetric random-walk interval-exit probabilities](../../../../../probability-theory-and-examples-fifth-edition-by-rick-durrett.md)

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
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

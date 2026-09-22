<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The precise conclusion is

$$
\boxed{\mathbb P\!\left(\lim_{n\to\infty}\frac{H_n}{n}=\frac23\right)=1.}
$$

To prove it, observe that the maximum rises exactly when the new height difference is positive:

$$
H_m-H_{m-1}=\mathbf1_{\{D_m>0\}}.
$$

A block landing in a shorter column produces $D_m=0$ and no rise; every other case raises the maximum and leaves $D_m>0$. Starting from $H_0=0$, telescoping gives

$$
\frac{H_n}{n}=\frac1n\sum_{m=1}^n\mathbf1_{\{D_m>0\}}.
$$

The difference chain is irreducible and positive recurrent by part (i). Apply the [countable-state Markov chain ergodic theorem](../../../../../countable-state-markov-chain-ergodic-theorem.md) to the bounded [indicator function](../../../../../indicator-function.md) $g(k)=\mathbf1_{\{k>0\}}$. Its stationary mean is $\sum_{k\geq1}\pi_k=1-\pi_0=2/3$, giving the asserted [almost sure convergence](../../../../../almost-sure-convergence.md). No [aperiodicity](../../../../../aperiodic-markov-chain.md) assumption is needed for this time average. This establishes the [growth rate of two-column sticky deposition](../../../../../growth-rate-of-two-column-sticky-deposition.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

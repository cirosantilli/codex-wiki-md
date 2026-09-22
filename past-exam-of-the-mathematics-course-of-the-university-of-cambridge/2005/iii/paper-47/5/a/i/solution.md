<h1 id="5/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Convergence means that the chain's distribution approaches the intended [posterior](../../../../../../../bayesian-posterior.md), independently of its initial state, under the relevant ergodicity assumptions. It is separate from obtaining enough effectively [independent](../../../../../../../independent-random-variables.md) draws for a precise answer. Start several chains at dispersed plausible points, examine [trace plots](../../../../../../../trace-plot.md) and stability of [posterior](../../../../../../../bayesian-posterior.md) summaries, compare between-chain and within-chain variation, and inspect [autocorrelation](../../../../../../../autocorrelation.md) and [effective sample size of a Markov chain](../../../../../../../effective-sample-size-of-a-markov-chain.md). Discard an initial transient when appropriate and report Monte Carlo uncertainty.

No finite diagnostic proves convergence. Agreement among chains started in the same basin can miss another mode. If different starting points give incompatible summaries, extend runs or improve proposals rather than merely deleting more observations. Extra thinning does not repair poor exploration; retaining all post-transient draws usually preserves more information for estimating uncertainty.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Paper 47](../../../../paper-47-split.md)
5. [Iii](../../../../split.md)
6. [2005](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

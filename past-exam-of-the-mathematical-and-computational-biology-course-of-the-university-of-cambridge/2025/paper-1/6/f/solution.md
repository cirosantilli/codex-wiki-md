<h1 id="6/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The trace has long, slowly changing stretches, indicating strong [autocorrelation](../../../../../autocorrelation.md) and poor exploration of the [posterior distribution](../../../../../bayesian-posterior.md). The reported [effective sample size of a Markov chain](../../../../../effective-sample-size-of-a-markov-chain.md) is only $36$, so the number of stored draws greatly exaggerates the information in the simulation. The [potential scale reduction factor](../../../../../potential-scale-reduction-factor.md) $\widehat R=1.21$ is appreciably above one and does not support convergence between chains. The reported [Monte Carlo standard error](../../../../../monte-carlo-standard-error.md) $0.04$ is also large relative to a posterior mean near $0.2$.

The exact [beta distribution](../../../../../beta-distribution.md) gives [posterior mean](../../../../../posterior-mean.md) $9/47\simeq0.19149$ and [standard deviation](../../../../../standard-deviation.md)

$$
\sqrt{\frac{9\cdot38}{47^2\cdot48}}\simeq0.0568,
$$

so the simulation's reported spread $0.11$ is another warning. Do not interpret its mean or interval estimates as reliable yet. Run multiple chains from dispersed starts, improve and tune the proposal or sampler, and use longer runs after adaptation. Recheck the traces, [potential scale reduction factor](../../../../../potential-scale-reduction-factor.md), and [effective sample size of a Markov chain](../../../../../effective-sample-size-of-a-markov-chain.md). More iterations help only if the chain actually explores its target well; thinning alone does not fix poor mixing.

## ↑ Ancestors (13)

1. [F](../f.md)
2. [6](../../6.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

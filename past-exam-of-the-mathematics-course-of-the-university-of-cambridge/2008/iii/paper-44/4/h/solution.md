<h1 id="4/h/solution">Solution</h1>

↑ **Parent:** [H](../h.md)

Model A has fifteen separate curve parameters plus one error-scale parameter. With such broad priors, one might have expected more of those sixteen parameters to be effectively estimated, rather than $p_D=12$, and might also have expected its greater unpooled flexibility to give better fit than the displayed $\overline D=248.1$. Model B instead has a smaller mean deviance despite sharing information between trees.

This is a diagnostic concern, not a mathematical impossibility. [Effective parameter count in DIC](../../../../../../effective-parameter-count-in-dic.md) depends on posterior curvature and parameterization, while mean posterior deviance is not minimized deviance. A weakly identified nonlinear asymptote–slope trade-off, skewness, multiple posterior regions or slow [Markov chain Monte Carlo](../../../../../../markov-chain-monte-carlo.md) mixing could explain the unexpected comparison. For A, the implied deviance at the posterior mean is $\overline D-p_D=236.1$; for B it is $230.3$. Inspect traces, effective sample sizes, independent chains and fitted curves, and extend sampling where needed. Fifty thousand iterations alone do not establish convergence.

## ↑ Ancestors (11)

1. [H](../h.md)
2. [4](../../4.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

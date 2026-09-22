<h1 id="26j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The proposal must connect the whole positive posterior support by moves with nonzero reverse probability. Use the full [Metropolis–Hastings acceptance probability](../../../../../../metropolis-hastings-acceptance-probability.md) for asymmetric proposals; dropping the reverse proposal factor generally targets the wrong distribution. Compute likelihoods and acceptance ratios on a logarithmic scale to avoid overflow and underflow, and handle zero weights explicitly. A lazy step prevents periodicity when distributional convergence is needed.

Finite-chain convergence does not guarantee a useful run length: separated modes and narrow bottlenecks can make mixing extremely slow. Tune proposals to explore efficiently, inspect several starting points and chains, and assess [autocorrelation](../../../../../../autocorrelation.md) and Monte Carlo uncertainty rather than treating correlated draws as independent observations. Discarding an initial segment can reduce initialization effects, but diagnostics do not prove that every posterior mode has been visited. Thinning is not required for correctness and often throws away useful information. The model and prior must themselves be specified correctly; an exact sampler from an incorrect posterior cannot repair the model.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [26J](../../26j.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

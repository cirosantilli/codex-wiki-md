<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The input vector $x$ contains the activities of presynaptic units or sensory features, and $w$ contains the corresponding synaptic weights. The linear output $y=w^Tx$ is their weighted sum; it may be a centered activity proxy rather than a literal nonnegative spike rate. The learning time scale is $\tau>0$, and take $\alpha>0$ for normalization. The term $yx$ is a [Hebbian learning](../../../../../../hebbian-learning.md) increment that strengthens weights correlated with the postsynaptic output. The term $-\alpha y^2w$ opposes unlimited growth.

For slow learning under stationary input statistics, average over inputs while holding the current weights fixed. Define $C=\langle xx^T\rangle$. The averaged [Oja's rule](../../../../../../oja-s-rule.md) is

$$
\tau\dot w=Cw-\alpha(w^TCw)w.
$$

Its squared norm obeys

$$
\boxed{\frac\tau2\frac{d\|w\|^2}{dt}=(w^TCw)(1-\alpha\|w\|^2).}
$$

Whenever the output second moment is positive, this drives the norm toward $1/\sqrt\alpha$, preventing the unbounded growth of an unconstrained Hebbian linear neuron. The direction becomes sensitive to dominant input correlations. Such a unit can learn a feature detector without supplied target labels, providing a simple mechanism for [unsupervised learning](../../../../../../unsupervised-learning.md) and [principal component analysis](../../../../../../principal-component-analysis.md). This averaged analysis assumes input fluctuations are fast relative to learning; it is not a claim that every individual stochastic update follows the same deterministic trajectory.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

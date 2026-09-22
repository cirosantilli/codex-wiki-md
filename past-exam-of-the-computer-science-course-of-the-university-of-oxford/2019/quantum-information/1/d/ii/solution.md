<h1 id="1/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the preparation and measurement from part (i). `RandomReset` returns the [density matrix](../../../../../../density-matrix-split.md) $\rho_R=(|0\rangle\langle0|+|1\rangle\langle1|)/2=I/2$, a [maximally mixed state](../../../../../../maximally-mixed-state.md). In the $|+\rangle,|-\rangle$ basis its two outcomes each have [probability](../../../../../../probability.md) $1/2$. In contrast, `RandomFlip` always gives outcome 0.

Guess `RandomFlip` after 0 and `RandomReset` after 1. With the supplied equal priors,

$$
\boxed{P_{\rm success}=\frac12\Pr(0\mid\texttt{RandomFlip})+\frac12\Pr(1\mid\texttt{RandomReset})=\frac12+\frac14=\frac34.}
$$

An outcome 1 identifies the reset action, but outcome 0 does not identify the flip action with certainty. For example, [Bayes' theorem](../../../../../../bayes-theorem.md) gives posterior [probability](../../../../../../probability.md) $2/3$ for the flip action after 0. The total success rate already accounts for the reset runs that also produce 0.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [1](../../../1.md)
4. [Quantum information](../../../../quantum-information-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)

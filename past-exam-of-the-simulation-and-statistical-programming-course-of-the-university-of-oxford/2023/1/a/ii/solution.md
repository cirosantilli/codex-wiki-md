<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Apply [Chebyshev's inequality](../../../../../chebyshev-s-inequality.md) to the [Monte Carlo estimator](../../../../../monte-carlo-estimator.md):

$$
\mathbb P\!\left(\left|\widehat\theta_n^{\mathrm{MC}}-\theta\right|\geq0.01\right)
\leq\frac{\operatorname{Var}(\widehat\theta_n^{\mathrm{MC}})}{0.01^2}
=\frac{10^4}{n}.
$$

Thus $10^4/n\leq0.01$ suffices, giving

$$
\boxed{n=1{,}000{,}000.}
$$

This is a finite-sample [probability](../../../../../probability.md) guarantee for every target satisfying the given [variance](../../../../../variance-split.md) assumption. It is a sufficient sample count supplied by the inequality, rather than a claim that every such target actually needs a million draws.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the simulation and statistical programming course of the University of Oxford](../../../../split.md)
6. [Simulation and statistical programming course of the University of Oxford](../../../../../simulation-and-statistical-programming-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

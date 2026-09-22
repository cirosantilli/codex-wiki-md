<h1 id="18h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The posterior expected loss at decision $\delta$ is

$$
R(\delta)
=2\int_{\gamma\leq\delta}(\delta-\gamma)\,dF(\gamma)
+\int_{\gamma>\delta}(\gamma-\delta)\,dF(\gamma).
$$

At continuity points its derivative is

$$
R'(\delta)=2F(\delta)-[1-F(\delta)]
=3F(\delta)-1.
$$

Thus the risk is minimized at a posterior one-third [quantile](../../../../../../quantile-function.md):

$$
\boxed{
\widehat\gamma_B=F^{-1}\left(\frac13\right)}.
$$

More generally, any $\delta$ satisfying

$$
F(\delta-)\leq\frac13\leq F(\delta)
$$

is optimal. The quantile lies below the posterior median, reflecting the smaller penalty assigned to underestimation.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [18H](../../18h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

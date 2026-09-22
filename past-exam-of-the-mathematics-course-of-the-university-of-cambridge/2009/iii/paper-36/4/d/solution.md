<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Under the independent-gene version of the model, integrating both component labels and effects gives

$$
\boxed{p(y\mid q,V)=\prod_{i=1}^N\{(1-q)f_0(y_i)+qf_1(y_i)\}.}
$$

This product uses independence of the gene effects and observation errors conditional on the shared parameters. Maximize its logarithm over $0\leq q\leq1$, for example with a one-dimensional bounded optimizer or a grid followed by refinement. Its derivatives are

$$
\ell'(q)=\sum_i\frac{f_1(y_i)-f_0(y_i)}{(1-q)f_0(y_i)+qf_1(y_i)},
\qquad
\ell''(q)=-\sum_i\frac{[f_1(y_i)-f_0(y_i)]^2}{[(1-q)f_0(y_i)+qf_1(y_i)]^2}\leq0.
$$

Thus the log [likelihood function](../../../../../../likelihood-function.md) is concave. An interior [maximum-likelihood estimate](../../../../../../maximum-likelihood-estimator.md) solves the score equation; otherwise it is at zero or one, determined by the endpoint score signs. An alternative [expectation-maximization algorithm](../../../../../../expectation-maximization-algorithm.md) iterates

$$
w_i=\frac{qf_1(y_i)}{(1-q)f_0(y_i)+qf_1(y_i)},\qquad
q_{\mathrm{new}}=\frac1N\sum_iw_i.
$$

For $V=0$, the components coincide and $q$ is not identifiable; for $V>0$ the full observation values carry information about the mixing fraction.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

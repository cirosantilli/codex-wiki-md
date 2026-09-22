<h1 id="o5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Ignoring a factor independent of the probabilities, the [likelihood function](../../../../likelihood-function.md) is $L(\pi)=\prod_i\pi_i^{n_i}$, so its log is $\ell(\pi)=\sum_i n_i\log\pi_i$ subject to $\sum_i\pi_i=1$. A [Lagrange multiplier](../../../../lagrange-multiplier.md) gives $n_i/\pi_i=\lambda$. Summing $\pi_i=n_i/\lambda$ makes $\lambda=n$.

Thus

$$
\boxed{\widehat\pi_i=n_i/n.}
$$

Since all counts are positive, a zero fitted cell [probability](../../../../probability.md) would have zero likelihood. On the interior the log-likelihood is strictly concave, so this stationary point is its unique global maximum.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [O5](../../o5.md)
3. [2013](../../../2013-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

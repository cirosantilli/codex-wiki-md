<h1 id="6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $Z$ be the unobserved part of the fourth count associated with the component of [probability](../../../../../../probability.md) $\theta/3$. Its complementary subcount has [probability](../../../../../../probability.md) $7/12$. Conditional on the observed fourth count and a parameter value,

$$
\boxed{Z\mid x_4,\theta\sim\operatorname{Bin}\left(x_4,\frac{4\theta}{7+4\theta}\right).}
$$

The complete-data [log-likelihood](../../../../../../log-likelihood.md) now has the simple form

$$
\ell_c(\theta)=(x_3+Z)\log\theta+(x_1+x_2)\log(1-\theta)
+\mathrm{constant}.
$$

The constant term can depend on the completed counts, but not on $\theta$. The split therefore converts the troublesome $\log(7+4\theta)$ term into a binomial-like maximization problem. Since $Z$ is unobserved, it should be averaged conditionally in an [EM algorithm](../../../../../../expectation-maximization-algorithm.md), not guessed or treated as observed.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

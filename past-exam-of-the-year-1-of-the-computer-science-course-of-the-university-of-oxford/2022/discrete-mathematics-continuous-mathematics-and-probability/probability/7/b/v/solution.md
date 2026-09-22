<h1 id="probability/7/b/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

By [linearity of expectation](../../../../../../../linearity-of-expectation.md), $\mathbb E N_n=np_n$. The [variance of a sum](../../../../../../../variance-of-a-sum.md) and the negative [covariance](../../../../../../../covariance.md) just proved give

$$
\operatorname{var}(N_n)=np_n(1-p_n)+n(n-1)(q_n-p_n^2)\le np_n(1-p_n)\le\frac n4.
$$

Apply [Chebyshev's inequality](../../../../../../../chebyshev-s-inequality.md) to the [empty-box indicators in uniform allocation](../../../../../../../empty-box-indicators-in-uniform-allocation.md):

$$
\boxed{\mathbb P\!\left(\left|\frac{N_n}{n}-p_n\right|>\epsilon\right)\le\frac{\operatorname{var}(N_n)}{n^2\epsilon^2}\le\frac1{4n\epsilon^2}\longrightarrow0.}
$$

This proves the required [concentration of the empty-box fraction](../../../../../../../concentration-of-the-empty-box-fraction.md). Since $p_n\to e^{-1}$, it also yields [convergence in probability](../../../../../../../convergence-in-probability.md) of $N_n/n$ to $e^{-1}$.

## ↑ Ancestors (14)

1. [V](../v.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Probability](../../../../probability.md)
5. [Discrete mathematics, continuous mathematics, and probability](../../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../../split.md)
8. [Year 1 of the computer science course of the University of Oxford](../../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
9. [Computer science course of the University of Oxford](../../../../../../../computer-science-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../../split.md)

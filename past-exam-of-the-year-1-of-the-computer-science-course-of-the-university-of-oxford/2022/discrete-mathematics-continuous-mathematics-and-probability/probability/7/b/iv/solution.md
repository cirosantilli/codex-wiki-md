<h1 id="probability/7/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $q_n=(1-2/n)^n$. The product of two distinct [empty-box indicators in uniform allocation](../../../../../../../empty-box-indicators-in-uniform-allocation.md) is the [indicator random variable](../../../../../../../indicator-random-variable.md) of both boxes being empty, so $\mathbb E(I_iI_j)=q_n$. Thus

$$
\boxed{\operatorname{cov}(I_i,I_j)=q_n-p_n^2=\left(1-\frac2n\right)^n-\left(1-\frac1n\right)^{2n}<0.}
$$

Indeed $0\le1-2/n<(1-1/n)^2$ for $n\ge2$, and taking the positive integer power $n$ preserves this strict inequality. This proves the negative [covariance](../../../../../../../covariance.md) directly.

## ↑ Ancestors (14)

1. [Iv](../iv.md)
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

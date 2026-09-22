# Concentration of the empty-box fraction

↑ **Parent:** [Uniform balls-in-bins allocation](uniform-balls-in-bins-allocation.md)

For $n$ balls in $n$ uniformly and independently chosen boxes, put $p_n=(1-1/n)^n$. The [empty-box indicators in uniform allocation](empty-box-indicators-in-uniform-allocation.md) have negative pairwise [covariance](covariance.md), so $\operatorname{var}(K_n)\le np_n(1-p_n)\le n/4$. [Chebyshev's inequality](chebyshev-s-inequality.md) gives

$$
\mathbb P(|K_n/n-p_n|>\epsilon)\le\frac1{4n\epsilon^2}\longrightarrow0.
$$

Since $p_n\to e^{-1}$, this proves the displayed [convergence in probability](convergence-in-probability.md). The centring and the negative [covariance](covariance.md) are essential to this short proof; an [expectation](expected-value-split.md) limit alone would not establish concentration.

## ↑ Ancestors (9)

1. [Uniform balls-in-bins allocation](uniform-balls-in-bins-allocation.md)
2. [Multinomial distribution](multinomial-distribution.md)
3. [Discrete probability distribution](discrete-probability-distribution-split.md)
4. [Probability distribution](probability-distribution-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/discrete-mathematics-continuous-mathematics-and-probability/probability/7/b/v/solution.md)

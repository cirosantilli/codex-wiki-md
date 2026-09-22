<h1 id="27j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume an identifiable smooth parametric model, an interior true parameter, a consistent interior [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md), interchange of differentiation and integration, a uniform local law of large numbers for the Hessian, and nonsingular finite [Fisher information](../../../../../../fisher-information-matrix.md). For one observation define the [score function](../../../../../../informant-function.md) $s_\theta(X)=\nabla_\theta\log p_\theta(X)$ and

$$
\boxed{J(\theta)=\mathbb E_\theta[s_\theta s_\theta^{\mathsf T}]
=-\mathbb E_\theta[\nabla_\theta^2\log p_\theta(X)]}.
$$

The [score function](../../../../../../informant-function.md) has expectation zero by differentiating the normalization of the density. Its sample sum satisfies $n^{-1/2}S_n(\theta)\xrightarrow d N(0,J)$ by the vector [central limit theorem](../../../../../../central-limit-theorem.md). The [score function](../../../../../../informant-function.md) equation and Taylor's formula give

$$
0=S_n(\theta)+\left[\int_0^1H_n(\theta+t(\widehat\theta_n-\theta))dt\right](\widehat\theta_n-\theta).
$$

The bracket divided by $n$ converges in probability to $-J$ by consistency and the assumed uniform law. Solving the equation and applying [Slutsky theorem](../../../../../../slutsky-theorem.md) yields

$$
\boxed{\sqrt n(\widehat\theta_n-\theta)\xrightarrow d N(0,J(\theta)^{-1})}.
$$

The integral Hessian avoids incorrectly assuming a single intermediate point for a vector-valued Taylor formula.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [27J](../../27j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

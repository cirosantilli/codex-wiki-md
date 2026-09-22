<h1 id="o/o4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [maximum-likelihood estimator](../../../../../maximum-likelihood-estimation-split.md) is a maximizer

$$
\widehat\theta\in\operatorname*{arg\,max}_{\theta}\ L_n(\theta),
\qquad L_n(\theta)=\prod_{i=1}^nf(X_i;\theta).
$$

Writing $\ell_n=\log L_n$ and the score $S_n=\nabla_\theta\ell_n$, the expected [Fisher information](../../../../../fisher-information-matrix.md) [matrix](../../../../../matrix.md) is

$$
\mathcal I_n(\theta)=\mathbb E_\theta[S_nS_n^T]
=-\mathbb E_\theta[\nabla_\theta^2\ell_n],
$$

where the equality uses the usual regularity conditions. For independent identically distributed observations, $\mathcal I_n=n\mathcal I_1$.

Under the standard identifiability, interior-parameter, [differentiability](../../../../../differentiability.md) and nonsingular-information assumptions, the large-sample distribution is

$$
\boxed{\sqrt n(\widehat\theta-\theta)\xrightarrow d
N(0,\mathcal I_1(\theta)^{-1}),}
$$

or approximately $\widehat\theta\sim N(\theta,\mathcal I_n(\theta)^{-1})$. Boundary parameters need not obey this regular approximation.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [O4](../../o4.md)
3. [O](../../../o.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

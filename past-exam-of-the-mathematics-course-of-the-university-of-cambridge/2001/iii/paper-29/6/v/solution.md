<h1 id="6/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

For independent families, multiply their [pedigree likelihoods](../../../../../../pedigree-likelihood.md). If family 1 has the known-phase counts above, the combined [log-likelihood](../../../../../../log-likelihood.md) derivative at an interior point is

$$
\ell'(\theta)=\frac{r_1}{\theta}-\frac{m_1-r_1}{1-\theta}+\frac{L_2'(\theta)}{L_2(\theta)}.
$$

Thus the [score equation for a phase-averaged linkage likelihood](../../../../../../score-equation-for-a-phase-averaged-linkage-likelihood.md) is

$$
\boxed{[r_1-m_1\widehat\theta]L_2(\widehat\theta)
+\widehat\theta(1-\widehat\theta)L_2'(\widehat\theta)=0.}
$$

For the general phase sum, let $w_s(\theta)=\pi_sC_s\theta^{r_s}(1-\theta)^{m_s-r_s}/L_2(\theta)$. Since the weights sum to one, the equivalent interior equation is

$$
\widehat\theta=\frac{r_1+\sum_sw_s(\widehat\theta)r_s}{m_1+\sum_sw_s(\widehat\theta)m_s}.
$$

The finite [likelihood](../../../../../../likelihood-function.md) sum is continuous on the compact parameter interval $[0,1/2]$, so a constrained maximum exists. This does not by itself prove an interior score root: complete nonrecombinant data, for example, maximize at zero. To show the requested root lies in the appropriate range for the two particular families, one must insert their transmission counts and evaluate the score or the resulting polynomial at the relevant endpoints.

**The source lacks those pedigree counts, so the data-specific equation and its asserted interior-root verification remain undetermined.** No universal interior-root claim is substituted for the missing calculation.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [6](../../6.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

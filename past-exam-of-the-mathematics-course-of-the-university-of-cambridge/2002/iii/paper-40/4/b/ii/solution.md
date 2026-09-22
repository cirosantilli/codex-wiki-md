<h1 id="4/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $\alpha_1=\alpha$, $\alpha_2=1-\alpha$, and introduce a categorical class label for each observation, encoded by $Z_{i1},Z_{i2}\in\{0,1\}$ with $Z_{i1}+Z_{i2}=1$. Its prior class [probability](../../../../../../../probability.md) is $\alpha_j$, and conditional on class $j$ the observation [probability density function](../../../../../../../probability-density-function.md) is $f_j(x_i)$. Thus its joint observation-label [probability density function](../../../../../../../probability-density-function.md) is

$$
p_\theta(x_i,Z_i)=\prod_{j=1}^2[\alpha_j f_j(x_i)]^{Z_{ij}}.
$$

Independence across observations yields the [finite Gaussian mixture with a common variance](../../../../../../../finite-gaussian-mixture-with-a-common-variance.md) complete-data [likelihood function](../../../../../../../likelihood-function.md)

$$
\boxed{L_c(\theta;x,Z)=\prod_{i=1}^n\prod_{j=1}^2[\alpha_j f_j(x_i)]^{Z_{ij}}.}
$$

Summing over the two possible labels at each observation recovers $\prod_i[\alpha f_1(x_i)+(1-\alpha)f_2(x_i)]$, the observed-data [likelihood function](../../../../../../../likelihood-function.md). The product requested in the PDF is therefore a joint complete-data [likelihood function](../../../../../../../likelihood-function.md). Strictly conditioning on $Z$ would remove the factors $\alpha_j$; the PDF's conditional notation for this joint product is imprecise.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 40](../../../../paper-40-split.md)
5. [Iii](../../../../split.md)
6. [2002](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Replace each [XY model](../../../../../../xy-model.md) bond weight by its periodic Gaussian approximation. With angles integrated using $d\theta/(2\pi)$, the [Villain model](../../../../../../villain-model.md) is

$$
\boxed{Z_V=(2\pi\beta)^{-N_b/2}\int\prod_x\frac{d\theta_x}{2\pi}
\sum_{\{n_{x,\mu}\in\mathbb Z\}}
\exp\left[-\frac1{2\beta}\sum_{x,\mu}n_{x,\mu}^2
+i\sum_{x,\mu}n_{x,\mu}(\theta_{x+\hat\mu}-\theta_x)\right],}
$$

where $N_b$ is the number of bonds. Changing the angle-measure normalization multiplies $Z_V$ by an explicit constant only. The [Poisson summation formula](../../../../../../poisson-summation-formula.md) applied to one bond gives the equivalent winding representation

$$
\frac1{\sqrt{2\pi\beta}}\sum_{n\in\mathbb Z}e^{-n^2/(2\beta)+in\psi}
=\sum_{p\in\mathbb Z}e^{-\beta(\psi-2\pi p)^2/2}.
$$

Thus the same [Villain model](../../../../../../villain-model.md) can be written $Z_V=\int\prod_xd\theta_x/(2\pi)\sum_{\{p_e\}}\exp[-\beta\sum_e(\Delta_e\theta-2\pi p_e)^2/2]$. The coefficient $1/\sqrt{2\pi\beta}$ is the PDF's value; the converted TeX incorrectly places $\beta$ outside the square root. The cosine-to-Gaussian replacement is a large-$\beta$ approximation, but the rest of the calculation treats $Z_V$ as the exact model for every positive $\beta$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

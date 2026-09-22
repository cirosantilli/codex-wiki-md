<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Every move can be drawn from a [full conditional distribution](../../../../../../full-conditional-distribution.md), producing a [Gibbs sampler](../../../../../../gibbs-sampler.md) with acceptance probability one. Write $s_{x,i}^2=\sigma_{x,i}^2$ and $s_{y,i}^2=\sigma_{y,i}^2$. First update independently

$$
\xi_i\mid-\sim N\!\left(
V_{\xi i}\left[\frac\mu{\tau^2}+\frac{\beta(\eta_i-\alpha)}{\sigma^2}+\frac{x_i}{s_{x,i}^2}\right],V_{\xi i}\right),
\quad
V_{\xi i}^{-1}=\frac1{\tau^2}+\frac{\beta^2}{\sigma^2}+\frac1{s_{x,i}^2},
$$

and then

$$
\eta_i\mid-\sim N\!\left(
V_{\eta i}\left[\frac{\alpha+\beta\xi_i}{\sigma^2}+\frac{y_i}{s_{y,i}^2}\right],V_{\eta i}\right),
\quad
V_{\eta i}^{-1}=\frac1{\sigma^2}+\frac1{s_{y,i}^2}.
$$

Let $X$ have rows $(1,\xi_i)$ and $\eta=(\eta_i)$. Update the [linear regression](../../../../../../linear-regression-split.md) coefficients jointly by

$$
\begin{pmatrix}\alpha\\\beta\end{pmatrix}\Bigm|-
\sim N_2\!\left((X^TX)^{-1}X^T\eta,
\sigma^2(X^TX)^{-1}\right),
$$

and update

$$
\mu\mid-\sim N\!\left(\bar\xi,\frac{\tau^2}{N}\right).
$$

Finally, the flat positive variance priors give the following full conditionals, each an [inverse-gamma distribution](../../../../../../inverse-gamma-distribution.md):

$$
\sigma^2\mid-\sim\operatorname{InvGamma}\!\left(\frac N2-1,
\frac12\sum_i(\eta_i-\alpha-\beta\xi_i)^2\right),
$$



$$
\tau^2\mid-\sim\operatorname{InvGamma}\!\left(\frac N2-1,
\frac12\sum_i(\xi_i-\mu)^2\right).
$$

A systematic sweep in the displayed order, using the newly sampled values immediately, defines the chain. The shapes are positive for $N>2$; full column rank of $X$ is also required.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

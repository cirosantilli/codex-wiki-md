<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $K_\theta$ have entries $k_\theta(t_i,t_j)$ and let

$$
C_\theta=K_\theta+\operatorname{diag}(\sigma_1^2,\ldots,\sigma_N^2).
$$

Independent Gaussian measurement errors give the [multivariate normal density](../../../../../../multivariate-normal-density.md)

$$
\boxed{
p(y\mid t;\mu,\theta)
=(2\pi)^{-N/2}|C_\theta|^{-1/2}
\exp\left[-\frac12(y-\mu\mathbf1)^TC_\theta^{-1}(y-\mu\mathbf1)\right]}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

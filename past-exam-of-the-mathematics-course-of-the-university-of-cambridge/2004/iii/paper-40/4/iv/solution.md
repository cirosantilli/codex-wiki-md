<h1 id="4/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For the standard [Cauchy distribution](../../../../../../cauchy-distribution.md) tail, use the indicator

$$
\boxed{\theta(x)=\mathbf1_{\{x\geq k\}}.}
$$

Then $\int\theta(x)f(x)\,dx$ is the desired [probability](../../../../../../probability.md), and the ordinary [importance sampling](../../../../../../importance-sampling.md) estimator is $n^{-1}\sum_i f(x_i)\mathbf1_{\{x_i\geq k\}}/g(x_i)$. The proposal must cover the nonzero integrand, namely the upper tail. A proposal restricted to $[0,k]$ cannot directly estimate this indicator [integral](../../../../../../integral.md); part (v) instead uses a complementary bounded-interval identity.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [4](../../4.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

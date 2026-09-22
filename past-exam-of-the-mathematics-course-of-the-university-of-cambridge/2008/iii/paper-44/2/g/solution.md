<h1 id="2/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

The gamma [full conditional distribution](../../../../../../full-conditional-distribution.md) has mean $(y_i+1)/(1+\psi)=(y_i+1)\phi$. The [tower property](../../../../../../law-of-total-expectation.md) and the [Beta distribution](../../../../../../beta-distribution.md) mean give

$$
\mathbb E[\theta_i\mid y]=(y_i+1)\frac{s}{s+n}.
$$

Writing $\overline y=s/n$ and $w=s/(s+n)=\overline y/(1+\overline y)$ yields

$$
\boxed{\mathbb E[\theta_i\mid y]=w y_i+(1-w)\overline y.}
$$

Thus [partial pooling](../../../../../../partial-pooling.md) pulls every local mean toward the overall sample mean. The common weight arises from the fixed shape-one mixing distribution; it is the [Poisson–exponential posterior shrinkage formula](../../../../../../poisson-exponential-posterior-shrinkage-formula.md).

## ↑ Ancestors (11)

1. [G](../g.md)
2. [2](../../2.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

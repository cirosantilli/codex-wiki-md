<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $I_X,I_Y$ be the original rates and $\mu_X,\mu_Y$ their unique zero points. Suppose first that $H<G$. At speed $b_n=n^{2(1-G)}$, the preceding argument gives X the rate zero at $\mu_X$ and infinity elsewhere, while Y retains $I_Y$. Independence allows the [product large-deviation principle](../../../../../../product-large-deviation-principle.md), and addition is continuous, so the [contraction principle for large deviations](../../../../../../contraction-principle-for-large-deviations.md) gives the sum rate

$$
K(z)=\inf_{x+y=z}\{I'_X(x)+I_Y(y)\}=I_Y(z-\mu_X).
$$

This is good, has unique zero $\mu_X+\mu_Y$, and inherits a strictly positive finite value by translation from $I_Y$. Thus the sum has [Hurstiness](../../../../../../hurstiness.md) G. The case $G<H$ is identical with the roles exchanged.

If $G=H$, the same product and contraction results apply to the original rates at their common speed, giving their [infimal convolution](../../../../../../infimal-convolution.md)

$$
K(z)=\inf_{x+y=z}\{I_X(x)+I_Y(y)\}.
$$

It is good. Every finite fiber [infimum](../../../../../../infimum.md) is attained: a minimizing sequence lies in a product of compact [sublevel sets](../../../../../../sublevel-set.md) and has a subsequence converging in the closed addition fiber. Consequently its only zero is $\mu_X+\mu_Y$. Choose $\hat x$ with $0<I_X(\hat x)<\infty$ and set $\hat z=\hat x+\mu_Y$. Then $\hat z$ differs from the zero point and $0<K(\hat z)\leq I_X(\hat x)<\infty$. The nondegeneracy requirement is therefore satisfied here too. In all cases,

$$
\boxed{\operatorname{Hurstiness}(X_n+Y_n)=\max(H,G).}
$$

The general results used are the independent product large-deviation theorem and the continuous contraction principle. Checking the zero set and a positive finite value is necessary in addition to obtaining an LDP.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

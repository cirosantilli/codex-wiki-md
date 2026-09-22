<h1 id="5j/solution">Solution</h1>

↑ **Parent:** [5J](../5j.md)

Expand the exponent in the [Inverse Gaussian distribution](../../../../../inverse-gaussian-distribution.md) with unit [shape parameter](../../../../../shape-parameter.md):

$$
-\frac{(x-\mu)^2}{2\mu^2x}
=-\frac{x}{2\mu^2}+\frac1\mu-\frac1{2x}.
$$

Consequently its [probability density function](../../../../../probability-density-function.md) can be written as

$$
f(x;\mu)=h(x)\exp\{\eta x-A(\eta)\},
$$

where

$$
h(x)=\frac1{\sqrt{2\pi x^3}}\exp\left(-\frac1{2x}\right),
\qquad
\eta=-\frac1{2\mu^2}<0,
\qquad
A(\eta)=-\sqrt{-2\eta}.
$$

Indeed, $-A(\eta)=\sqrt{-2\eta}=1/\mu$. This is the canonical form of a one-parameter [exponential family](../../../../../exponential-family-split.md), and its [natural parameter](../../../../../natural-parameter-of-an-exponential-family.md) is therefore

$$
\boxed{\eta=-\frac1{2\mu^2}}.
$$

Here the natural statistic is $T(X)=X$. The [exponential-family derivative identities](../../../../../exponential-family-derivative-identities.md) give

$$
\mathbb E_\eta X=A'(\eta)=(-2\eta)^{-1/2}=\mu
$$

and

$$
\operatorname{var}_\eta X=A''(\eta)=(-2\eta)^{-3/2}=\mu^3.
$$

Thus

$$
\boxed{\mathbb E X=\mu,
\qquad \operatorname{var}X=\mu^3}.
$$

## ↑ Ancestors (10)

1. [5J](../5j.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

By [Poisson-gamma conjugacy](../../../../../../poisson-gamma-conjugacy.md), the [posterior density](../../../../../../posterior-density.md) is proportional to

$$
\lambda^{a-1}e^{-b\lambda}\lambda^n e^{-T\lambda}
=\lambda^{a+n-1}e^{-(b+T)\lambda}.
$$

Thus **the shape-rate posterior is**

$$
\boxed{\lambda\mid\mathcal D\sim\operatorname{Gamma}(A,B),\quad A=a+n,\quad B=b+T.}
$$

Its [posterior mean](../../../../../../posterior-mean.md) is $A/B$ and its [variance](../../../../../../variance-split.md) is $A/B^2$. The parameter $B$ is a rate, rather than a scale.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Under equal costs for either wrong assignment, the [Bayes classifier](../../../../../../bayes-classifier.md) chooses the class of greatest [posterior probability](../../../../../../posterior-probability.md). With positive prior probabilities, it assigns class one when $\pi_1f_1(x)>\pi_2f_2(x)$; ties can be resolved arbitrarily. For the two [multivariate normal densities](../../../../../../multivariate-normal-density.md) with common positive-definite [covariance matrix](../../../../../../covariance-matrix.md) $V$, their normalizing factors cancel. The log posterior odds are

$$
\begin{aligned}
\log\frac{\pi_1f_1(x)}{\pi_2f_2(x)}
&=\log\frac{\pi_1}{\pi_2}-\frac12\big[(x-\mu_1)^TV^{-1}(x-\mu_1)-(x-\mu_2)^TV^{-1}(x-\mu_2)\big]\\
&=(\mu_1-\mu_2)^TV^{-1}x-\frac12(\mu_1^TV^{-1}\mu_1-\mu_2^TV^{-1}\mu_2)+\log\frac{\pi_1}{\pi_2}.
\end{aligned}
$$

Therefore the [Gaussian Bayes classifier](../../../../../../gaussian-bayes-classifier.md) has the required linear form, with

$$
\boxed{a=V^{-1}(\mu_1-\mu_2),\qquad b=\frac12(\mu_1+\mu_2)^TV^{-1}(\mu_1-\mu_2)-\log\frac{\pi_1}{\pi_2}.}
$$

A larger prior probability for class one decreases $b$, expanding its decision region. The [prior-dependent Gaussian discriminant boundary](../../../../../../prior-dependent-gaussian-discriminant-boundary.md) is the hyperplane $a^Tx=b$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

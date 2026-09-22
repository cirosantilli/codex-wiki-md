<h1 id="4/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Put $c_i=\int_D\varphi_i(x)\,d\lambda_n(x)$. The stated scalar random variable is

$$
Z=\int_DU(x)\,d\lambda_n(x)
=\sum_{i=1}^k\sqrt{\nu_i}\,c_i\xi_i.
$$

As a finite [linear combination of independent normal random variables](../../../../../../linear-combination-of-independent-normal-random-variables.md), it is normally distributed. Its mean is zero and its variance is

$$
\boxed{\operatorname{Var}(Z)
=\frac12\sum_{i=1}^k\nu_i
\left(\int_D\varphi_i\,d\lambda_n\right)^2}.
$$

Finally, [orthonormality](../../../../../../orthonormal-set.md) of the $\varphi_i$ gives

$$
\|U\|_X^2=\sum_{i=1}^k\nu_i\xi_i^2.
$$

Since $\mathbb E\xi_i^2=1/2$,

$$
\boxed{\int_\Omega\|U\|_X^2\,d\mathbb P
=\frac12\sum_{i=1}^k\nu_i}.
$$

## ↑ Ancestors (11)

1. [3](../3.md)
2. [4](../../4.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

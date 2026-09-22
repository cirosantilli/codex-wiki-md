<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

After [integration by parts](../../../../../../integration-by-parts.md), define the Euclidean quadratic operator

$$
K[\lambda]=-partial_\tau^2-v^2\nabla^2+i\lambda.
$$

The action can then be written as

$$
S=\frac1{2vg}\sum_{a=1}^N
\langle n_a,K[\lambda]n_a\rangle
-\frac{iN}{2vg}\int d^2x\,d\tau\,\lambda.
$$

Each component of $\mathbf n$ gives the same bosonic [Gaussian functional integral](../../../../../../gaussian-functional-integral.md), so

$$
\int\mathcal D\mathbf n\,
e^{-\frac1{2vg}\sum_a\langle n_a,Kn_a\rangle}
\propto(\det K)^{-N/2}.
$$

Discarding a $\lambda$-independent normalization, the remaining [functional determinant](../../../../../../functional-determinant.md) gives

$$
\boxed{
Z=\int\mathcal D\lambda\,e^{-\widetilde S[\lambda]},
\qquad
\widetilde S[\lambda]
=\frac N2\operatorname{Tr}\log K[\lambda]
-\frac{iN}{2vg}\int d^2x\,d\tau\,\lambda.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 337](../../../paper-337-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

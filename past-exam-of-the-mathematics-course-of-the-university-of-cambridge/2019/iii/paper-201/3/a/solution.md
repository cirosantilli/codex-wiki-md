<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Since $X_1$ is uniform on $\{-1,1\}$,

$$
\psi(\lambda)
=\log\mathbb E[e^{\lambda X_1}]
=\log\left(\frac{e^\lambda+e^{-\lambda}}2\right)
=\log\cosh\lambda.
$$

For $|x|<1$, the supremum in the [Legendre transform of a cumulant-generating function](../../../../../../legendre-transform-of-a-cumulant-generating-function.md) is attained where

$$
x=\psi'(\lambda)=\tanh\lambda,
\qquad
\lambda=\frac12\log\frac{1+x}{1-x}.
$$

Substitution gives the [Rademacher large-deviation rate function](../../../../../../rademacher-large-deviation-rate-function.md)

$$
\boxed{\psi^*(x)
=\frac{(1+x)\log(1+x)+(1-x)\log(1-x)}2}
$$

for $|x|\leq1$, with $0\log0=0$; it is $+\infty$ for $|x|>1$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

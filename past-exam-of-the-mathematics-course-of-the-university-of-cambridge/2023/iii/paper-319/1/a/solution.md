<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [C0-semigroup](../../../../../../c0-semigroup.md) on a [Banach space](../../../../../../banach-space-split.md) $X$ is a family $U(t)\in\mathcal B(X)$ such that

$$
U(0)=I,
\qquad
U(t+s)=U(t)U(s),
\qquad
\lim_{t\downarrow0}U(t)x=x
$$

for every $x\in X$. Its [infinitesimal generator of a semigroup](../../../../../../infinitesimal-generator-of-a-semigroup.md) is

$$
Ax=\lim_{t\downarrow0}\frac{U(t)x-x}{t},
$$

with [generator domain](../../../../../../generator-domain.md)

$$
D(A)=\left\{x\in X:
\lim_{t\downarrow0}\frac{U(t)x-x}{t}
\text{ exists in }X\right\}.
$$

For $M\geq1$ and $\omega\in\mathbb R$, write $A\in\mathcal G(M,\omega)$ when $A$ generates a $C_0$-semigroup satisfying $\|U(t)\|\leq Me^{\omega t}$. The [Hille-Yosida theorem](../../../../../../hille-yosida-theorem.md) states that this holds exactly when $A$ is closed and densely defined,

$$
(\omega,\infty)\subset\rho(A),
$$

and, for every real $\lambda>\omega$ and every integer $n\geq1$,

$$
\boxed{
\|R(\lambda,A)^n\|
\leq\frac{M}{(\lambda-\omega)^n}},
\qquad
R(\lambda,A)=(\lambda I-A)^{-1}.
$$

The estimates for every resolvent power, rather than only $n=1$, are essential when $M>1$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 319](../../../paper-319-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

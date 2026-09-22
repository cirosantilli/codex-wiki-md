<h1 id="28k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $\lambda_i=z|V_i|$. Then

$$
N(V_i)\sim\operatorname{Pois}(\lambda_i),
\qquad
\mathbb E N(V_i)=\lambda_i,
$$

and $\lambda_i\to\infty$. The [Poisson central limit theorem](../../../../../../poisson-central-limit-theorem.md) gives

$$
\frac{N(V_i)-\lambda_i}{\sqrt{\lambda_i}}
\xrightarrow{\mathrm d}N(0,1).
$$

Since $\sqrt{\lambda_i}=\sqrt z\,\sqrt{|V_i|}$,

$$
\frac{N(V_i)-\mathbb E N(V_i)}{\sqrt{|V_i|}}
=\sqrt z\,
\frac{N(V_i)-\lambda_i}{\sqrt{\lambda_i}}
\xrightarrow{\mathrm d}\boxed{N(0,z)}.
$$

Equivalently, the [characteristic function](../../../../../../characteristic-function.md) of the left-hand side is

$$
\exp\left\{
\lambda_i\left(
e^{it/\sqrt{|V_i|}}-1-\frac{it}{\sqrt{|V_i|}}
\right)\right\}
\longrightarrow e^{-zt^2/2},
$$

which is the characteristic function of that centered [normal distribution](../../../../../../normal-distribution.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [28K](../../28k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

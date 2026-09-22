<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $U=X/\sigma$. The standardized efficient [score function](../../../../../../informant-function.md) for scale is

$$
\Lambda(u)=-1-u\frac{f'(u)}{f(u)}.
$$

An optimal B-robust scale M-estimator solves

$$
\sum_{i=1}^n\psi(X_i/\widehat\sigma)=0,
$$

where the optimal bounded score has the clipped-score form

$$
\psi(u)=\operatorname{clip}\bigl(A\{\Lambda(u)-z\},-b,b\bigr).
$$

The constants $A,z$ enforce [Fisher consistency](../../../../../../fisher-consistency.md), the chosen normalization, and the clipping bound $b$ on the [influence function](../../../../../../influence-function.md).

For the [standard normal distribution](../../../../../../standard-normal-distribution.md), $f'(u)/f(u)=-u$, hence $\Lambda(u)=u^2-1$. The score therefore simplifies to

$$
\psi(u)=\operatorname{clip}\bigl(A(u^2-1-z),-b,b\bigr),
$$

with $z$ chosen so that $\mathbb E\psi(Z)=0$ for $Z\sim N(0,1)$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 223](../../../paper-223-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

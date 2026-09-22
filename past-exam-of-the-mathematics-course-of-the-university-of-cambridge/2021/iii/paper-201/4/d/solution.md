<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

At the meeting time,

$$
A_T^+=A_T^-=\frac{C_T}{\sqrt2}.
$$

The process $C$ is independent of $T$, so conditional on $T=u$ the meeting position is $N(0,u/2)$. Independently, $B_t-B_u$ is $N(0,t-u)$. Therefore

$$
Z_t\mid\{T=u\}\sim N(0,t-u/2).
$$

For $0<s\leq t$, integrate this conditional [Gaussian distribution](../../../../../../normal-distribution.md) against the density from part c:

$$
\boxed{
\mathbb P(T\leq s,\ Z_t\leq z)
=\int_0^s
\Phi\left(\frac z{\sqrt{t-u/2}}\right)
\frac a{\sqrt{\pi u^3}}e^{-a^2/u}\,du.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

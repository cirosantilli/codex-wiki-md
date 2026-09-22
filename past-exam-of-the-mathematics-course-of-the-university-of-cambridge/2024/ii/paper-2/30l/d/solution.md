<h1 id="30l/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Given $0<z<1$, take

$$
w=\frac{1+\sqrt{1-z^2}}z>1,
\qquad z=\frac2{w+w^{-1}}.
$$

Choose $A,B$ so that

$$
Aw^{-a}+Bw^a=1,\qquad
Aw^b+Bw^{-b}=1.
$$

Solving,

$$
A=\frac{w^a-w^{-b}}{w^{a+b}-w^{-(a+b)}},
\qquad
B=\frac{w^b-w^{-a}}{w^{a+b}-w^{-(a+b)}}.
$$

The stopped discounted martingale is bounded, and $T$ is finite, so part (b) gives

$$
A+B=\mathbb E\!\left[
z^T(Aw^{X_T}+Bw^{-X_T})\right]=\mathbb E(z^T).
$$

Therefore the [discounted symmetric random-walk exit transform](../../../../../../discounted-symmetric-random-walk-exit-transform.md) is

$$
\boxed{
\mathbb E(z^T)=
\frac{w^a+w^b-w^{-a}-w^{-b}}
{w^{a+b}-w^{-(a+b)}}},
\qquad
w=\frac{1+\sqrt{1-z^2}}z.
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [30L](../../30l.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

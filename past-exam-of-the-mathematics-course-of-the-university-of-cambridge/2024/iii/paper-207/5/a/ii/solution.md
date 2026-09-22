<h1 id="5/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The transformation is $T_k=a_kU_k^b$. Because $U_k$ has a unit-rate [exponential distribution](../../../../../../../exponential-distribution.md),

$$
S_k(t)=\mathbb P\!\left(U_k>(t/a_k)^{1/b}\right)
=\exp\!\left[-(t/a_k)^{1/b}\right].
$$

Thus $T_k$ has a [Weibull distribution](../../../../../../../weibull-distribution.md), with

$$
H_k(t)=(t/a_k)^{1/b},
\qquad
h_k(t)=\frac1b a_k^{-1/b}t^{1/b-1}.
$$

**Consequently $h_2(t)/h_1(t)=(a_1/a_2)^{1/b}$ is constant, proving [proportional hazards](../../../../../../../proportional-hazards-model.md).**

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

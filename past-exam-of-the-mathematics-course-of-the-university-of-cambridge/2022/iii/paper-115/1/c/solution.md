<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Fix $I$ and write $I'$ for the complementary column indices. Over $U_I$, decompose $M=(M_I,M_{I'})$ and $v=(v_I,v_{I'})$. The equation $Mv=0$ is equivalent to

$$
v_I=-M_I^{-1}M_{I'}v_{I'}.
$$

Matrix inversion is [smooth](../../../../../../smooth-function.md) on the [invertible matrices](../../../../../../invertible-matrix.md), so

$$
(M,u)\longmapsto\left(M,\bigl(-M_I^{-1}M_{I'}u,u\bigr)\right)
$$

is a smooth, fiberwise-linear trivialization $U_I\times\mathbb R^{n-m}\to\pi^{-1}(U_I)$. The sets $U_I$ cover the base, proving that $\pi:E_{m,n}\to X_{m,n}$ is a [vector bundle](../../../../../../vector-bundle.md) of rank $n-m$. It is the [kernel bundle of a constant-rank family of linear maps](../../../../../../kernel-bundle-of-a-constant-rank-family-of-linear-maps.md), and its rank also follows from the [rank-nullity theorem](../../../../../../rank-nullity-theorem.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 115](../../../paper-115-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

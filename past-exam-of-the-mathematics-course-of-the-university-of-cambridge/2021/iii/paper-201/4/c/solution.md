<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Apply the orthogonal transformation

$$
D_t=\frac{A_t^+-A_t^-}{\sqrt2},
\qquad
C_t=\frac{A_t^++A_t^-}{\sqrt2}.
$$

The processes $D$ and $C$ are independent one-dimensional Brownian motions, with $D_0=\sqrt2a$ and $C_0=0$. The meeting time is the first time $D$ hits zero, which is almost surely finite by one-dimensional Brownian recurrence.

The [Brownian reflection principle](../../../../../../reflection-principle-wiener-process.md) gives the first-passage density from $x>0$ to zero as

$$
\frac{x}{\sqrt{2\pi u^3}}e^{-x^2/(2u)}.
$$

Substituting $x=\sqrt2a$ gives the [meeting time of two independent Brownian motions](../../../../../../meeting-time-of-two-independent-brownian-motions.md) density

$$
\boxed{f_T(u)=\frac a{\sqrt{\pi u^3}}e^{-a^2/u}},
\qquad u>0.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
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

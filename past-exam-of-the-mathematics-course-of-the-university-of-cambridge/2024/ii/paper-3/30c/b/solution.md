<h1 id="30c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The endpoint $t=0$ is treated by rotating onto its [method of steepest descent](../../../../../../method-of-steepest-descent.md) ray. It contributes

$$
\Gamma(3/2)(-ix)^{-3/2}=\frac{\sqrt\pi}{2}(-ix)^{-3/2}.
$$

At $t=1$, put $s=1-t$ and expand

$$
(1-s)^{1/2}=\sum_{n=0}^\infty(-1)^n\binom{1/2}{n}s^n.
$$

Termwise endpoint integration, using $\int_0^\infty s^ne^{-ixs}ds=n!(ix)^{-n-1}$ on the rotated ray, gives

$$
I(x)\sim\frac{\sqrt\pi}{2}(-ix)^{-3/2}
-e^{ix}\sum_{n=0}^\infty a_n(-ix)^{-n-1},
$$

where

$$
a_n=n!\binom{1/2}{n}.
$$

The two displayed contributions come from the two endpoints; the remaining deformed contour is exponentially or algebraically smaller after any fixed truncation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [30C](../../30c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

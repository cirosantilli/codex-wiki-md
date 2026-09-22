<h1 id="30a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Complete the square: $z^2-2iz=(z-i)^2+1$. The pole of $(1-iz)^{-1}$ is at $z=-i$, so the contour may be shifted upward through the [saddle point](../../../../../../saddle-point.md) $z=i$ without crossing a singularity. Setting $z=t+i$ gives the exact steepest-descent representation

$$
I(x)=e^{-x}\int_{-∞}^{∞}{e^{-xt^2}\over2-it}\,dt.
$$

Near the saddle,

$$
{1\over2-it}=\sum_{n\geq0}{(it)^n\over2^{n+1}}.
$$

Odd terms integrate to zero, while

$$
\int_{-∞}^{∞}t^{2m}e^{-xt^2}\,dt=Γ(m+1/2)x^{-m-1/2}.
$$

The [Watson lemma](../../../../../../watson-s-lemma.md) therefore yields the full [asymptotic expansion](../../../../../../asymptotic-expansion.md)

$$
\boxed{I(x)\sim e^{-x}\sum_{m=0}^{∞}{(-1)^mΓ(m+1/2)\over2^{2m+1}x^{m+1/2}}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [30A](../../30a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

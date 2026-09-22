<h1 id="4g/solution">Solution</h1>

↑ **Parent:** [4G](../4g.md)

**Rouché's theorem.** Suppose $f,g$ are [holomorphic functions](../../../../../holomorphic-function.md) on a neighbourhood of the closure of a bounded domain enclosed by a simple, positively oriented, piecewise smooth curve. If $|g(z)|<|f(z)|$ on the boundary, then $f$ and $f+g$ have the same number of zeros inside, counted with [multiplicity](../../../../../multiplicity-mathematics.md).

Apply [Rouche theorem](../../../../../rouche-s-theorem.md) with $f(z)=z^4+3$ and $g(z)=e^{iz}$ on the first-quadrant quarter-disc of radius $R=\sqrt2$. On the two radial segments, $z^4$ is nonnegative real, so $|f|\geq3$, whereas $|g|=e^{-\operatorname{Im}z}\leq1$. On the circular arc,

$$
|f(z)|\geq|z|^4-3=1.
$$

At every arc point with positive imaginary part, $|g|<1$, giving the strict inequality; at the remaining endpoint $z=R$, $|f|=7>1=|g|$. Thus the strict boundary inequality holds everywhere, including the origin.

The four zeros of $f$ have modulus $3^{1/4}$ and arguments $\pi/4,3\pi/4,5\pi/4,7\pi/4$. Exactly one lies inside the chosen domain. [Rouche theorem](../../../../../rouche-s-theorem.md) gives exactly one zero of $f+g$ there, counted with [multiplicity](../../../../../multiplicity-mathematics.md), so that zero is simple. Finally any zero in the open first quadrant satisfies

$$
|z|^4=|3+e^{iz}|\leq3+e^{-\operatorname{Im}z}<4.
$$

There can be no additional zero outside the quarter-disc. Hence

$$
\boxed{\text{Exactly one zero lies in the first quadrant, and }|z_0|<\sqrt2.}
$$

## ↑ Ancestors (10)

1. [4G](../4g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

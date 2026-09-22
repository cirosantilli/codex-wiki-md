<h1 id="3b/solution">Solution</h1>

↑ **Parent:** [3B](../3b.md)

A convenient version of [Rouché's theorem](../../../../../rouche-s-theorem.md) is: if $f,g$ are [holomorphic functions](../../../../../holomorphic-function.md) on a neighbourhood of a closed [disk](../../../../../disk-mathematics.md), and $|g|<|f|$ on its boundary, then $f$ and $f+g$ have the same number of [zeros](../../../../../zero-of-a-function.md), counted with [multiplicity](../../../../../multiplicity-mathematics.md), in the disk. In particular neither has a boundary zero under this comparison.

Put $F_a(z)=z^4-a(z-1)(z^2-1)-1/2$ and use the boundary $|z|=\sqrt2$. There $|z^4|=4$, $1\le|z^2-1|\le3$, and $\sqrt2-1\le|z-1|\le\sqrt2+1$.

For $a=1/3$, compare with $z^4$:

$$
\left|\frac13(z-1)(z^2-1)+\frac12\right|\le\sqrt2+\frac32<4.
$$

Therefore [Rouché's theorem](../../../../../rouche-s-theorem.md) gives four [zeros](../../../../../zero-of-a-function.md).

For $a=12$, compare with $-12(z-1)(z^2-1)$:

$$
|z^4-1/2|\le\frac92<12(\sqrt2-1)\le12|z-1||z^2-1|.
$$

The comparison polynomial is $-12(z-1)^2(z+1)$, which has three [zeros](../../../../../zero-of-a-function.md) in the disk, counting the double zero at $1$.

For $a=5$, take $G(z)=(z^2-1)(z-2)(z-3)$. Expansion gives $F_5=G+1/2$. On the boundary,

$$
|G|\ge(2-\sqrt2)(3-\sqrt2)=8-5\sqrt2>\frac12.
$$

The last strict inequality follows from $3/2>\sqrt2$. Only the simple [zeros](../../../../../zero-of-a-function.md) $1,-1$ of $G$ lie inside the disk. Thus, in the requested order,

$$
\boxed{4,\quad3,\quad2.}
$$

## ↑ Ancestors (10)

1. [3B](../3b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

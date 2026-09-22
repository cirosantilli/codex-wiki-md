<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a fixed [prime](../../../../../../prime-number.md) $p\in[P,2P]$, the grid $a/p$ has [circular spacing](../../../../../../circular-spacing.md) $1/p\geq1/(2P)$. Consequently an arc of length $\Delta=1/P$ contains at most three points of this grid, including endpoints. The standard [Chebyshev estimate](../../../../../../chebyshev-estimate.md) $\pi(t)\ll t/\log t$ for the [prime-counting function](../../../../../../prime-counting-function.md) gives

$$
K(1/P)\leq3\#\{p\in[P,2P]:p\text{ prime}\}\ll\frac P{\log P}.
$$

Since $N\leq P$, the [local-multiplicity large sieve](../../../../../../local-multiplicity-large-sieve.md) yields the [prime-denominator large sieve](../../../../../../prime-denominator-large-sieve.md):

$$
\boxed{\sum_{\substack{P\leq p\leq2P\\p\text{ prime}}}\sum_{a=1}^{p-1}|S(a/p)|^2\ll\frac{P^2}{\log P}E.}
$$

By contrast, distinct [reduced fractions](../../../../../../reduced-fraction.md) with denominators at most $2P$ have circular distance at least $1/(4P^2)$: their difference, even after subtraction of an [integer](../../../../../../integer.md), has a nonzero [integer](../../../../../../integer.md) numerator over denominator $pp\prime$. Applying part (a) alone gives only $(4P^2+2\pi N)E\ll P^2E$. **The local-multiplicity argument saves a factor of $\log P$.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

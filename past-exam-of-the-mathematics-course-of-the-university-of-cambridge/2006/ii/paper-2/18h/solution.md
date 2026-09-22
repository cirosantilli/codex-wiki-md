<h1 id="18h/solution">Solution</h1>

↑ **Parent:** [18H](../18h.md)

Begin with two points at distance one. A ruler draws the line through two known points; a compass draws a circle with a known centre and a constructible radius. New points are intersections of such lines and circles. A [real number](../../../../../real-number.md) is constructible when it occurs as a coordinate of a point obtained by finitely many such operations; a complex point is constructible when both coordinates are.

If current coordinates lie in a [field](../../../../../field.md) $K\subseteq\mathbb R$, a line-line intersection solves [linear equations](../../../../../linear-equation.md) over $K$, while line-circle or circle-circle intersections reduce to a [quadratic equation](../../../../../quadratic-equation.md) over $K$. Thus each step requires at most adjoining a [square root](../../../../../square-root.md). Consequently every [constructible number](../../../../../constructible-number.md) lies in a tower

$$
\mathbb Q=K_0\subseteq K_1\subseteq\cdots\subseteq K_m,\qquad [K_{i+1}:K_i]\le2.
$$

Conversely [field](../../../../../field.md) sums and differences are obtained by laying off segments, products and quotients by similar triangles, and a positive [square root](../../../../../square-root.md) by the geometric-mean construction in a semicircle. Hence every [real number](../../../../../real-number.md) in such a tower is constructible. This proves the quadratic-tower criterion, not merely its necessity.

In particular a constructible [algebraic number](../../../../../algebraic-number.md) has degree a power of two. Degree alone is not sufficient in general; the exact criterion is containment in a quadratic tower. Equivalently the [Galois group](../../../../../galois-group.md) of its [normal closure](../../../../../normal-closure.md) is a finite two-group: a tower's [normal closure](../../../../../normal-closure.md) remains a two-extension, and a two-group admits a chain of subgroups with successive index two, yielding the converse by [Galois correspondence](../../../../../galois-correspondence.md).

The standard impossibility results follow. Doubling a unit-volume cube requires $\sqrt[3]2$, whose [polynomial](../../../../../polynomial-split.md) $X^3-2$ is irreducible by Eisenstein and has degree three. Trisecting an arbitrary angle would in particular trisect $60$ degrees, requiring $2\cos20^\circ$, a root of $X^3-3X-1$. This cubic has no rational root and is irreducible, so this construction is impossible, although some particular angles can be trisected. Squaring the [unit circle](../../../../../complex-unit-circle.md) requires side length $\sqrt\pi$, impossible because $\pi$ is transcendental whereas [constructible numbers](../../../../../constructible-number.md) are algebraic.

For a regular $n$-gon, constructibility is equivalent to that of $e^{2\pi i/n}$. The cyclotomic extension is Galois of degree $\varphi(n)$, so it is constructible exactly when this degree is a power of two. Writing the [prime factorization](../../../../../fundamental-theorem-of-arithmetic.md) of $n$ shows the equivalent condition

$$
\boxed{n=2^a p_1\cdots p_s,\quad p_i\text{ distinct Fermat primes}.}
$$

Indeed [odd prime](../../../../../odd-prime.md) exponents must be one, and each $p_i-1$ must be a power of two. If $2^m+1$ is [prime](../../../../../prime-number.md), $m$ must itself be a power of two by factoring when $m$ has an odd divisor. Conversely this factorization makes the cyclotomic [Galois group](../../../../../galois-group.md) a two-group and provides a quadratic tower. This gives both positive constructions, such as the regular seventeen-gon, and obstructions, such as the regular seven-gon.

## ↑ Ancestors (10)

1. [18H](../18h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

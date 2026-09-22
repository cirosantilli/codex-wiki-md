<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For an [odd prime](../../../../odd-prime.md) $p$, [Euler's criterion](../../../../euler-s-criterion.md) states

$$
\boxed{a^{(p-1)/2}\equiv\left(\frac ap\right)\pmod p.}
$$

For $p\nmid a$, the [Legendre symbol](../../../../legendre-symbol.md) is $1$ for a [quadratic residue](../../../../quadratic-residue-split.md) and $-1$ for a [quadratic nonresidue](../../../../quadratic-nonresidue.md); if $p\mid a$, both sides are zero.

The product is a single power because the [arithmetic progression](../../../../arithmetic-progression.md) of exponents has sum $2017\cdot2018/2$:

$$
\prod_{j=1}^{2017}2^j=2^{2017\cdot1009}.
$$

Since $2017\equiv1\pmod8$, the [second supplementary law for quadratic reciprocity](../../../../second-supplementary-law-for-quadratic-reciprocity.md) gives $(2/2017)=1$. Hence [Euler's criterion](../../../../euler-s-criterion.md) gives $2^{1008}\equiv1\pmod{2017}$. Reduce the exponent using $1009=1008+1$ and $2017=2\cdot1008+1$:

$$
2^{2017\cdot1009}\equiv2^{2017}
=2(2^{1008})^2\equiv2\pmod{2017}.
$$

The least nonnegative [remainder](../../../../remainder.md) is therefore **$2$**.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the short options course of the University of Oxford](../../../split.md)
5. [Short options course of the University of Oxford](../../../../short-options-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

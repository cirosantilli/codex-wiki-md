<h1 id="38c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Dahlquist equivalence theorem](../../../../../../dahlquist-equivalence-theorem.md) states that a linear multistep method is convergent for well-posed sufficiently smooth initial-value problems, with consistent starting values, if and only if it is consistent and zero-stable. Zero-stability means that every root of its first characteristic polynomial lies in the closed unit disk, with roots on the unit circle simple.

Here the characteristic polynomials are

$$
\rho(z)=z^3+(2a-3)z^2-(2a-3)z-1=(z-1)[z^2+2(a-1)z+1],\qquad\sigma(z)=a(z^2+z).
$$

Consistency holds because $\rho(1)=0$ and $\rho'(1)=\sigma(1)=2a$. The two remaining roots have product one. For $0<a<2$ they are distinct conjugate unit roots, and neither equals one. At $a=0$, the root one is triple; at $a=2$, the root minus one is double. Outside $[0,2]$, the remaining roots are real reciprocal roots and one has modulus greater than one. Thus

$$
\boxed{\text{convergence holds exactly for }0<a<2.}
$$

The order conditions give $c_2=0$ and $c_3=6-a$, which is nonzero throughout the convergent range. Therefore **the order of convergence is exactly two**, for starting approximations of matching accuracy.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [38C](../../38c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

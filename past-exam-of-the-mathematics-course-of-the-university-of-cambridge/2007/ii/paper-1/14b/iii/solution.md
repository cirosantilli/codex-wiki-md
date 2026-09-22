<h1 id="14b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Because $b$ is not an integer, the coefficient $\sin(\pi b)$ is nonzero. The expression of $B$ in terms of the [entire](../../../../../../entire-function.md) function $J$ can therefore have poles only at integral $z$, and at most simple ones. Positive integers are removable: $B(z,b)$ is already analytic there for $\operatorname{Re}b>0$, and [analytic continuation](../../../../../../analytic-continuation.md) in $b$ gives

$$
B(n,b)=\frac{(n-1)!}{b(b+1)\cdots(b+n-1)}\qquad(n\ge1).
$$

Thus $J$ vanishes at those integers, cancelling the denominator zero. The [Gamma function](../../../../../../gamma-function.md) formula $B(z,b)=\Gamma(z)\Gamma(b)/\Gamma(z+b)$ identifies the remaining singularities:

$$
\boxed{z=-m\ (m=0,1,\ldots),\qquad
\operatorname{Res}_{z=-m}B(z,b)=\frac{(-1)^m\Gamma(b)}{m!\Gamma(b-m)}.}
$$

For nonintegral $b$, these residues are nonzero, so every listed singularity is a genuine simple pole.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [14B](../../14b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

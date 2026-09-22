<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [strong maximum principle for subharmonic functions](../../../../../../strong-maximum-principle-for-subharmonic-functions.md) is: on a connected open domain, the canonical [upper semicontinuous](../../../../../../upper-semicontinuity.md) representative of a subharmonic function cannot attain a finite global maximum at an interior point unless it is constant. A local maximum instead forces constancy on an appropriate neighbourhood; it alone does not assert constancy on the whole domain unless that value is a global maximum.

Suppose $u\leq M$ on $\Omega$ and $u(x_0)=M$. For every sufficiently small ball centred at $x_0$, the subharmonic mean inequality gives

$$
M=u(x_0)\leq\frac1{|B_r|}\int_{B_r(x_0)}u\leq M.
$$

The nonnegative function $M-u$ has integral zero, so $u=M$ almost everywhere on that ball. Its canonical representative is then $M$ at every point of the ball, by taking still smaller local averages.

The maximum set $E=\{x:u(x)=M\}$ is consequently open by the same argument at each of its points. It is closed relative to $\Omega$, because upper semicontinuity makes its complement $\{u<M\}$ open. It is nonempty, and [connectedness](../../../../../../connected-space.md) gives $E=\Omega$. Therefore **$u\equiv M$**. This proves the principle, including its representative and [connectedness](../../../../../../connected-space.md) hypotheses. Arbitrary representatives do not satisfy it: the function equal to zero almost everywhere but assigned value one at the origin has zero distributional Laplacian and an artificial pointwise maximum.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

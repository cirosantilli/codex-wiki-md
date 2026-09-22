<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a [holomorphic function](../../../../../holomorphic-function.md) $h:\mathbb D\to\mathbb D$, the [Schwarz-Pick lemma](../../../../../schwarz-pick-theorem.md) states

$$
\left|\frac{h(z)-h(a)}{1-\overline{h(a)}h(z)}\right|
\leq\left|\frac{z-a}{1-\overline a z}\right|,
\qquad
\frac{|h'(a)|}{1-|h(a)|^2}\leq\frac1{1-|a|^2}.
$$

Equality in the first inequality for distinct points, or in the derivative inequality at one point, occurs exactly when $h$ is an [automorphism of the unit disk](../../../../../automorphism-of-the-unit-disk.md).

Here is a proof, including the underlying [Schwarz lemma](../../../../../schwarz-lemma.md). If $u:\mathbb D\to\mathbb D$ is [holomorphic](../../../../../complex-differentiability-at-a-point.md) and $u(0)=0$, then $u(z)/z$ has a removable singularity at zero. On $|z|=r<1$ its modulus is at most $1/r$. The [maximum modulus principle](../../../../../maximum-modulus-principle.md) on this circle, followed by $r\uparrow1$, gives $|u(z)|\leq|z|$ and $|u'(0)|\leq1$. Equality at a nonzero point, or $|u'(0)|=1$, forces $u(z)/z$ to be a constant of modulus one by the same [maximum modulus principle](../../../../../maximum-modulus-principle.md).

Set $\phi_a(z)=(z-a)/(1-\overline a z)$, an [automorphism of the unit disk](../../../../../automorphism-of-the-unit-disk.md). The composite $\phi_{h(a)}\circ h\circ\phi_a^{-1}$ fixes zero. The [Schwarz lemma](../../../../../schwarz-lemma.md) gives the first inequality, while its derivative at zero gives the second. The equality conclusion follows because a composite attaining equality is a rotation. Conversely, every [automorphism of the unit disk](../../../../../automorphism-of-the-unit-disk.md) attains equality. This also proves contraction of the [hyperbolic metric](../../../../../hyperbolic-metric.md).

The boundary lower bound first guarantees a zero inside the unit circle. If $f(0)=0$, there is nothing to prove about existence. Otherwise, if $f$ had no zeros on the closed [unit disc](../../../../../unit-disc.md), $1/f$ would be [holomorphic](../../../../../complex-differentiability-at-a-point.md) on a neighborhood of it and satisfy $|1/f|\leq1/A$ on the boundary. The [maximum modulus principle](../../../../../maximum-modulus-principle.md) would give $|f(0)|\geq A$, contradicting the hypothesis. The boundary lower bound excludes boundary zeros, so there is a zero $a$ with $|a|<1$.

The upper boundary bound and the [maximum modulus principle](../../../../../maximum-modulus-principle.md) give $|f|\leq B$ on the unit circle and its interior. The function is nonconstant under the stated hypotheses, so $f/B$ takes its interior values in the open [unit disc](../../../../../unit-disc.md). Apply the [Schwarz-Pick lemma](../../../../../schwarz-pick-theorem.md) to the points $a$ and $0$:

$$
\boxed{|a|\geq\frac{|f(0)|}{B}.}
$$

This is the [zero location bound from Schwarz-Pick](../../../../../zero-location-bound-from-schwarz-pick.md), and it applies to every zero inside the unit circle.

The bound is sharp. Given $0<a<1$ and $B>0$, choose

$$
f(z)=B\frac{z-a}{1-az},\qquad 1<R<1/a.
$$

This [holomorphic function](../../../../../holomorphic-function.md) has no pole in $\mathbb D_R$, has constant modulus $B$ on the unit circle, and satisfies $|f(0)|=Ba<B$. With $A=B$, its zero at $a$ gives equality. The case $a=0$ is also attained by $f(z)=Bz$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 5](../../paper-5-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

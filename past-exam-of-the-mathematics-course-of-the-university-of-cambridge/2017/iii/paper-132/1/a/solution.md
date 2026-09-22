<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix $z_0\in\mathcal U$. We prove the [Riemann mapping theorem](../../../../../../riemann-mapping-theorem.md) in this case by maximizing a normalized [derivative](../../../../../../derivative.md). Choose $a\notin\mathcal U$. Since $\mathcal U$ is a [simply connected domain](../../../../../../simply-connected-domain.md) and $z-a$ never vanishes, it has a [holomorphic square root](../../../../../../holomorphic-square-root.md) $g$. This $g$ is [injective](../../../../../../injective-function.md), and $g(\mathcal U)$ is disjoint from $-g(\mathcal U)$: equality up to sign would first force the original points to coincide. Choose $b\in g(\mathcal U)$ and $r>0$ with $B(b,r)\subset g(\mathcal U)$. The ball $B(-b,r)$ is omitted, so $1/(g+b)$ is a bounded [univalent function](../../../../../../univalent-function.md). Scaling and composing with an [automorphism of the unit disk](../../../../../../automorphism-of-the-unit-disk.md) produces an [injective](../../../../../../injective-function.md) [holomorphic function](../../../../../../holomorphic-function.md) $\phi:\mathcal U\to\mathbb D$ with $\phi(z_0)=0$ and $\phi'(z_0)>0$.

Let $\mathcal F$ be the family of all such normalized [univalent functions](../../../../../../univalent-function.md). A [Cauchy estimate](../../../../../../cauchy-estimate.md) in a small disk about $z_0$ bounds their [derivatives](../../../../../../derivative.md), so $M=\sup_{\phi\in\mathcal F}\phi'(z_0)$ is finite and positive. Choose a maximizing sequence in this [normal family](../../../../../../normal-family.md). [Montel theorem](../../../../../../montel-s-theorem.md) gives a subsequence converging uniformly on [compact](../../../../../../compact-space.md) subsets to $\phi$. Its [derivative](../../../../../../derivative.md) at $z_0$ is $M>0$. The [maximum modulus principle](../../../../../../maximum-modulus-principle.md) puts its image in $\mathbb D$, and [Hurwitz's theorem](../../../../../../hurwitz-s-theorem.md) implies that a nonconstant limit of [injective](../../../../../../injective-function.md) [holomorphic functions](../../../../../../holomorphic-function.md) is [injective](../../../../../../injective-function.md). Thus the maximum is attained.

If $a_1\in\mathbb D$ is omitted, then $a_1\ne0$. Put $T_a(w)=(w-a)/(1-\overline a w)$. A [holomorphic square root](../../../../../../holomorphic-square-root.md) $v$ of $T_{a_1}\circ\phi$ exists, is [injective](../../../../../../injective-function.md), and takes values in $\mathbb D$. Compose $v$ with $T_{v(z_0)}$ and a rotation to normalize it. Writing $s=|a_1|\in(0,1)$, the new [derivative](../../../../../../derivative.md) has magnitude

$$
M\frac{1-s^2}{2\sqrt s(1-s)}
=M\frac{1+s}{2\sqrt s}>M,
$$

a contradiction. Therefore $\phi$ maps onto $\mathbb D$. The [Cayley transform between the half-plane and disk](../../../../../../cayley-transform-between-the-half-plane-and-disk.md) now gives

$$
\boxed{f(z)=i\,\frac{1+\phi(z)}{1-\phi(z)}:\mathcal U\xrightarrow{\sim}\mathbb H,\qquad
\operatorname{Im}f(z)=\frac{1-|\phi(z)|^2}{|1-\phi(z)|^2}>0.}
$$

Its inverse is [holomorphic](../../../../../../complex-differentiability-at-a-point.md) by the [holomorphic inverse function theorem](../../../../../../holomorphic-inverse-function-theorem.md), so this is a [biholomorphism](../../../../../../biholomorphism.md). The proper-subset hypothesis was used to choose $a\notin\mathcal U$; the whole [complex plane](../../../../../../complex-plane.md) cannot be mapped this way, by [Liouville theorem](../../../../../../liouville-theorem.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 132](../../../paper-132-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

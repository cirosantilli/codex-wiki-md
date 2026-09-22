<h1 id="23f/solution">Solution</h1>

↑ **Parent:** [23F](../23f.md)

The [uniformization theorem](../../../../../uniformization-theorem.md) states that every simply connected [Riemann surface](../../../../../riemann-surfaces.md) is [biholomorphic](../../../../../biholomorphism.md) to exactly one of the [Riemann sphere](../../../../../riemann-sphere.md) $\widehat{\mathbb C}$, the [complex plane](../../../../../complex-plane.md) $\mathbb C$, or the [unit disc](../../../../../unit-disc.md) $\mathbb D$. A surface is uniformized by one of these when that surface is its universal cover. The only surface uniformized by $\widehat{\mathbb C}$ is the sphere itself, because every nonidentity Möbius transformation has a fixed point and therefore cannot act as a deck transformation. The [Riemann surfaces uniformized by the complex plane](../../../../../riemann-surfaces-uniformized-by-the-complex-plane.md) are

$$
\boxed{\mathbb C,\qquad\mathbb C^*,\qquad
\mathbb C/\Lambda\text{ for a lattice }\Lambda.}
$$

Let $U\subseteq\mathbb C$ have a complement containing at least two points. Its universal cover cannot be the sphere because $U$ is noncompact. If it were the plane, the covering map $\mathbb C\to U\hookrightarrow\mathbb C$ would be a nonconstant [entire function](../../../../../entire-function.md) omitting two values, contrary to the [Little Picard theorem](../../../../../little-picard-theorem.md). The [plane domain with two omitted points is hyperbolic](../../../../../plane-domain-with-two-omitted-points-is-hyperbolic.md), so

$$
\boxed{U\text{ is uniformized by }\mathbb D.}
$$

Now put $S=R\setminus\{P_1,\ldots,P_n\}$. The spherical possibility occurs only for $(g,n)=(0,0)$. By the preceding list, the plane-uniformized possibilities are

$$
(g,n)=(0,1),(0,2),(1,0),
$$

which give respectively $2g-2+n=-1,0,0$. Every remaining pair has $2g-2+n>0$ and must have disc universal cover. Thus the [uniformization of a punctured compact Riemann surface](../../../../../uniformization-of-a-punctured-compact-riemann-surface.md) gives

$$
\boxed{
\begin{aligned}
S\text{ is uniformized by }\mathbb D
&\Longleftrightarrow 2g-2+n>0,\\
S\text{ is uniformized by }\mathbb C
&\Longleftrightarrow 2g-2+n\in\{-1,0\}.
\end{aligned}}
$$

For the [complex torus](../../../../../complex-torus.md) $X=\mathbb C/\Lambda$, any analytic map $f:\mathbb C\to X$ lifts through the [universal covering map](../../../../../universal-cover.md) to an entire function $F:\mathbb C\to\mathbb C$. If $F$ is constant, so is $f$. Otherwise Little Picard says that $F$ omits at most one complex number. For every $x\in X$, its lifts form an infinite coset $z+\Lambda$, so at least one lift is attained by $F$. Hence the [holomorphic map from the complex plane to a one-dimensional complex torus](../../../../../holomorphic-map-from-the-complex-plane-to-a-one-dimensional-complex-torus.md) satisfies

$$
\boxed{f\text{ is constant or surjective}.}
$$

Finally, $\mathbb C$ and $\mathbb D$ are homeomorphic by

$$
z\longmapsto\frac{z}{1+|z|},
\qquad
w\longmapsto\frac{w}{1-|w|}.
$$

They are not [conformally equivalent](../../../../../conformal-equivalence.md): a biholomorphism $\mathbb C\to\mathbb D$ would be a nonconstant bounded entire function, contradicting the [Liouville theorem](../../../../../liouville-theorem.md). This proves the claimed example of [complex plane and unit disc are homeomorphic but not conformally equivalent](../../../../../complex-plane-and-unit-disc-are-homeomorphic-but-not-conformally-equivalent.md).

## ↑ Ancestors (10)

1. [23F](../23f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

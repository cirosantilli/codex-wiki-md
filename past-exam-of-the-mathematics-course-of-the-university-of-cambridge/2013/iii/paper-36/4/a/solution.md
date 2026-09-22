<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Interpret the angle as the [directed subspace angle](../../../../../../directed-subspace-angle.md) defined by the infimum of projected unit [vectors](../../../../../../vector.md); it is different from the [smallest angle between two subspaces](../../../../../../smallest-angle-between-two-subspaces.md). Write

$$
a=\cos\theta_{W,V^\perp}>0,\qquad b=\cos\theta_{V^\perp,W}>0.
$$

Consider the [bounded linear operator](../../../../../../continuous-linear-operator.md) $T:W\longrightarrow V^\perp$ given by $Tw=P_{V^\perp}w$. Its [adjoint operator](../../../../../../adjoint-operator.md), between these two [Hilbert spaces](../../../../../../hilbert-space-split.md), is $T^*u=P_Wu$: for $w\in W$ and $u\in V^\perp$, the [orthogonal projections](../../../../../../orthogonal-projection.md) give $\langle Tw,u\rangle=\langle w,u\rangle=\langle w,P_Wu\rangle$. The two positive [directed subspace angle](../../../../../../directed-subspace-angle.md) cosines yield

$$
\|Tw\|\ge a\|w\|,\qquad\|T^*u\|\ge b\|u\|.
$$

The first bound makes $T$ [injective](../../../../../../injective-function.md) and gives a closed range. Explicitly, if $Tw_j$ converges, then $\|w_j-w_k\|\le a^{-1}\|Tw_j-Tw_k\|$, so $(w_j)$ is a [Cauchy sequence](../../../../../../cauchy-sequence.md). The [closed subspace of a Hilbert space](../../../../../../closed-subspace-of-a-hilbert-space.md) $W$ is complete, and its limit maps to the proposed range limit. The second bound gives $\ker T^*=\{0\}$. A [vector](../../../../../../vector.md) $u\in V^\perp$ orthogonal to the range has $T^*u=0$, so it must be zero. The range is therefore dense as well as closed in $V^\perp$, and $T$ is onto. This is the mechanism of [invertibility from lower bounds on an operator and its adjoint](../../../../../../invertibility-from-lower-bounds-on-an-operator-and-its-adjoint.md).

For any $f\in H$, choose the unique $w\in W$ with $Tw=P_{V^\perp}f$. Then $P_{V^\perp}(f-w)=0$, so $f-w\in V$. Moreover, if $w\in W\cap V$, then $Tw=0$ and hence $w=0$. **Every vector has a unique decomposition, and**

$$
\boxed{H=W\oplus V.}
$$

The [direct sum](../../../../../../direct-sum.md) is a topological one as well: the component $w=T^{-1}P_{V^\perp}f$ depends boundedly on $f$, with [operator norm](../../../../../../operator-norm.md) at most $a^{-1}$.

For precision, the quoted equality of the norms of complementary [oblique projections](../../../../../../oblique-projection.md) needs both summands nonzero. For example, with $H=\mathbb R$, $V=H$ and $W=\{0\}$, the [oblique projection](../../../../../../oblique-projection.md) is $I$, so $\|I\|=1$ but $\|I-I\|=0$. The [secant function](../../../../../../secant-trigonometry.md) has value one here, so the second equality in the quoted formula fails. With nonzero complementary summands its intended version is valid. The proof above does not use that formula. The angle itself is undefined on a zero source space because it has no unit [vectors](../../../../../../vector.md); expressing the hypotheses as the two lower bounds handles zero spaces without ambiguity.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

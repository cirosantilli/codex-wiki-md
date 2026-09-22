<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the fact that [infinite cyclic subgroups of hyperbolic groups are undistorted](../../../../../../infinite-cyclic-subgroups-of-hyperbolic-groups-are-undistorted.md): if $z$ has infinite order in a [hyperbolic group](../../../../../../hyperbolic-group.md), then its [stable word length](../../../../../../stable-word-length.md)

$$
\tau(z)=\lim_{m\to\infty}\frac{|z^m|}{m}
$$

is strictly positive. The limit exists by subadditivity and the [Fekete lemma](../../../../../../fekete-s-lemma.md). It is invariant under [conjugation](../../../../../../conjugation.md), because conjugating $z^m$ changes its length by at most twice the conjugator's length. It also satisfies $\tau(z^k)=|k|\tau(z)$.

In the given [Baumslag-Solitar group](../../../../../../baumslag-solitar-group.md), $b$ has infinite order. To verify this without presuming the presentation's normal form, let $a$ act on the real line by $t\mapsto3t$ and $b$ by $t\mapsto t+1$. These affine bijections satisfy $aba^{-1}=b^3$, and every nonzero power of $b$ is a nonidentity translation. Thus the element $b$ in the presented group cannot have finite order.

If an injective [group homomorphism](../../../../../../group-homomorphism.md) to $G$ existed, its images $z$ of $b$ and $u$ of $a$ would satisfy $uzu^{-1}=z^3$, with $z$ still of infinite order. Consequently

$$
\tau(z)=\tau(uzu^{-1})=\tau(z^3)=3\tau(z),
$$

forcing $\tau(z)=0$, a contradiction. Therefore

$$
\boxed{\text{There is no injective homomorphism }\operatorname{BS}(1,3)\to G.}
$$

Equivalently, the relation gives $a^kba^{-k}=b^{3^k}$, so powers of $z$ with exponent $3^k$ would have length at most $2k|u|+|z|$. This contradicts the linear lower bound for an undistorted infinite cyclic subgroup. This alternative also makes the exponential compression obstruction explicit.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 133](../../../paper-133-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

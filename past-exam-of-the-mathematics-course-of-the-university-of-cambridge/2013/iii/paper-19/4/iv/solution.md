<h1 id="4/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $\kappa=(\omega_2)^M$ be the fixed ground [ordinal](../../../../../../ordinal.md). We prove that $S$ remains stationary in this [ordinal](../../../../../../ordinal.md). The [chain condition for forcing](../../../../../../chain-condition-for-forcing.md) ensures that $\kappa$ remains regular: possible values of each coordinate of an ordinal-valued name form a ground set of size less than $\kappa$, by a maximal deciding [forcing antichain](../../../../../../forcing-antichain.md). A hypothetical cofinal map with domain below $\kappa$ would have its range covered by fewer than $\kappa$ such small sets, hence bounded by regularity in $M$.

Let $\dot C$ name a [club set](../../../../../../club-set.md) in $\kappa$, and take $p\in G$ [forcing](../../../../../../forcing-split.md) this. For each $\alpha<\kappa$, choose in $M$ a maximal [forcing antichain](../../../../../../forcing-antichain.md) above $p$ deciding the least point of $\dot C$ strictly above $\alpha$. Its set of possible values has size less than $\kappa$, so choose a ground bound $h(\alpha)<\kappa$ larger than all of them. The ground set

$$
D=\{\delta<\kappa:\delta\text{ is limit and }(\forall\alpha<\delta)\ h(\alpha)<\delta\}
$$

is a [club set](../../../../../../club-set.md) by the usual countable closure iteration and regularity. For every $\delta\in D$, $p$ forces $\dot C\cap\delta$ unbounded in $\delta$, and closedness forces $\delta\in\dot C$. Hence $p\Vdash\check D\subseteq\dot C$. In $M$, choose $\delta\in S\cap D$; that same [ordinal](../../../../../../ordinal.md) belongs to $S\cap C$ in the extension. **Stationarity at the fixed ground $\kappa$ is preserved.**

There is an important qualification to the printed $\omega_2$ notation. If it is recomputed internally as $(\omega_2)^{M[G]}$, the assertion is false without preservation of smaller [cardinals](../../../../../../cardinal-number.md). Finite partial maps from $\omega$ to $(\omega_1)^M$ form a [forcing](../../../../../../forcing-split.md) of size $(\aleph_1)^M$, hence have the $(\aleph_2)^M$-chain condition, but collapse $(\omega_1)^M$ to countable. Then $(\omega_2)^M=(\omega_1)^{M[G]}$, while $(\omega_2)^{M[G]}$ is larger. The old $S$ is bounded in this new $\omega_2$, so cannot be stationary there. The proved statement uses the fixed ground [ordinal](../../../../../../ordinal.md), or alternatively requires the lower-cardinal preservation needed to retain its aleph index.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [4](../../4.md)
3. [Paper 19](../../../paper-19-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

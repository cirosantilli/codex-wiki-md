<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

First prove the [torsion in an HNN extension](../../../../../torsion-in-an-hnn-extension.md) statement directly from [Britton's lemma](../../../../../britton-s-lemma.md). Let $z$ have finite order in an [HNN extension](../../../../../hnn-extension.md) of $G$. Among its conjugates, choose a reduced normal-form word with the smallest possible number $k$ of [stable letters](../../../../../stable-letter.md). If $k=0$, that conjugate lies in the embedded base $G$, so its finite order and the base's [torsion-free group](../../../../../torsion-free-group.md) property force it to be the identity.

Suppose instead that $k>0$. There are no internal [pinches in an HNN extension](../../../../../pinch-in-an-hnn-extension.md) because the word is reduced. There is also no pinch at the join of its end with its beginning. Indeed, write it as $g_0t^{\varepsilon_1}g_1\cdots t^{\varepsilon_k}g_k$ and conjugate off $g_0$ to obtain $t^{\varepsilon_1}g_1\cdots t^{\varepsilon_k}(g_kg_0)$. If the joined subword $t^{\varepsilon_k}(g_kg_0)t^{\varepsilon_1}$ were a pinch, its two signs would be opposite; conjugating by $t^{\varepsilon_1}$ and using the pinch relation would reduce the stable-letter count by two, contradicting minimality. Thus every positive power is reduced with exactly $rk$ stable letters in the $r$th power. [Britton's lemma](../../../../../britton-s-lemma.md) makes every such power nonidentity, contradicting finite order. We have proved

$$
\boxed{G\text{ torsion-free}\quad\Longrightarrow\quad\text{every HNN extension of }G\text{ is torsion-free}.}
$$

The base embeds by the same lemma, so finite order has not been lost or artificially introduced by a quotient.

For the [countable torsion-free embedding with two conjugacy classes](../../../../../countable-torsion-free-embedding-with-two-conjugacy-classes.md), start with $G_0=G$. Given a countable torsion-free $G_j$, list all ordered pairs $(a,b)$ of its nonidentity elements. Both elements have infinite order, so the assignment $a^r\mapsto b^r$ is an isomorphism between their infinite [cyclic subgroups](../../../../../cyclic-subgroup.md). Successively adjoin one stable letter for each pair with relation $t_{a,b}^{-1}at_{a,b}=b$. Each [HNN extension](../../../../../hnn-extension.md) embeds the previous group and is torsion-free by the result just proved. Let $G_{j+1}$ be the union after all pairs from $G_j$ have been treated. It remains countable because only countably many generators were added, and torsion-free because any element and any purported finite-order equation occur in a finite stage.

Repeat this whole process: new stable letters and their products must also be included in later pair lists. In the final increasing union

$$
\boxed{\widehat G=\bigcup_{j\geq0}G_j,}
$$

the original $G$ embeds and torsion-freeness and countability persist. Any two nonidentity elements lie together in some $G_j$ and are conjugate in $G_{j+1}$. Thus **every countable torsion-free group embeds in a countable torsion-free group in which all nonidentity elements are conjugate**. If the initial group is nontrivial there are exactly two [conjugacy classes](../../../../../conjugacy-class.md); for the trivial group the stated condition is vacuous, or one can begin with $\mathbb Z$ instead. The listing is set-theoretic; no algorithm for recognizing nonidentity elements is assumed.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 1](../../paper-1-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

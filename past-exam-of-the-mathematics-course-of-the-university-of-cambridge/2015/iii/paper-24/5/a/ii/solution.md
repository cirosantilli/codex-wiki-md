<h1 id="5/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**For an arbitrary ground model, this alternative needs an additional arithmetic hypothesis.** The requested countable-cover property already prevents any collapse of an infinite ground-model cardinal. If a cardinal $\theta$ were collapsed, there would be a surjection $f:\alpha\to\theta$ with $|\alpha|^M<\theta$. The asserted ground-model $F$ would cover $\theta$ by the union of $|\alpha|^M$ countable sets, a ground-model set of size at most $\max(\aleph_0,|\alpha|^M)<\theta$, a contradiction. Thus all infinite cardinals are preserved.

Put $\lambda=(\aleph_3)^M$, which must then remain $\aleph_3$. If the extension has continuum $\lambda$, it has

$$
\lambda^{\aleph_0}=(2^{\aleph_0})^{\aleph_0}=\lambda.
$$

The ground-model functions from $\omega$ into $\lambda$ remain present and their cardinality cannot be collapsed. Necessarily

$$
\boxed{M\models\lambda^{\aleph_0}=\lambda.}
$$

For example, a ground model with continuum larger than $\aleph_3$ cannot satisfy the printed request. This is a genuine missing hypothesis, rather than a forcing construction that works for every $M$.

Under the necessary hypothesis, use [Cohen forcing](../../../../../../../cohen-forcing.md) to add $\lambda$ reals:

$$
\mathbb P=\operatorname{Fn}(\lambda\times\omega,2,{<}\omega).
$$

The [delta-system lemma](../../../../../../../delta-system-lemma.md) shows that it has the [countable chain condition for forcing](../../../../../../../countable-chain-condition-for-forcing.md): an uncountable family of finite conditions has an uncountable subfamily whose domains form a delta-system and whose values agree on its root, so any two of that subfamily are compatible. It therefore preserves cardinals. Its $\lambda$ coordinate reals are pairwise distinct by dense disagreement requirements. Conversely each [nice forcing name](../../../../../../../nice-forcing-name.md) for a real uses countably many countable [antichains in a forcing order](../../../../../../../antichain-in-a-forcing-order.md), so the number of such names is at most $\lambda^{\aleph_0}=\lambda$. Hence

$$
\boxed{M[G]\models2^{\aleph_0}=\aleph_3.}
$$

For any ordinal-valued function name, choose for each $\xi<\alpha$ a maximal [antichain in a forcing order](../../../../../../../antichain-in-a-forcing-order.md) deciding its value. The [countable chain condition for forcing](../../../../../../../countable-chain-condition-for-forcing.md) makes the set $F(\xi)$ of possible ordinal values countable in $M$. Pad it with $\omega$ if needed to make it countably infinite. The [possible-values lemma for chain-condition forcing](../../../../../../../possible-values-lemma-for-chain-condition-forcing.md) gives the stronger pointwise covering statement

$$
\boxed{f(\xi)\in F(\xi)\quad(\xi<\alpha),}
$$

which implies the requested range inclusion. When a condition only forces that the name is such a function, make these choices below that condition; it belongs to the generic filter witnessing the actual function.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Paper 24](../../../../paper-24-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

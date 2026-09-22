<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $D_\alpha,D_\beta$ be the disjoint complete meridian-disk system of $H_1$, and let $D_\gamma,D_\delta$ be that of $H_2$. The identification $\phi(\alpha)=\gamma$ joins $D_\alpha$ and $D_\gamma$ into an embedded sphere $S$ in $M$. Each disk is nonseparating in its [handlebody](../../../../../../handlebody.md): cutting along it leaves a genus-one [handlebody](../../../../../../handlebody.md), and cutting along the other then gives a ball. After cutting $M$ along $S$, the two cut [handlebodies](../../../../../../handlebody.md) are connected and are still joined along the complement of the common boundary circle. Hence $S$ is nonseparating.

Cap the two new sphere boundaries with balls. The resulting [closed manifold](../../../../../../closed-manifold.md) $N$ inherits a genus-one [Heegaard splitting](../../../../../../heegaard-splitting.md): its two sides are the [solid tori](../../../../../../solid-torus.md) obtained by cutting the original [handlebodies](../../../../../../handlebody.md) along their common disks. Their meridians are the surviving curves $\beta$ and $\delta$. The hypothesis that $\phi(\beta)$ avoids $\gamma$ makes it descend to the compressed torus, and its single intersection with $\delta$ remains a single intersection there.

A genus-one splitting whose two meridians intersect once is $S^3$. To see this directly, choose the target torus basis $(\mu,\lambda)$ with $\mu$ its meridian. The other meridian is $a\mu\pm\lambda$. A meridional [Dehn twist](../../../../../../dehn-twist.md), extending across the target [solid torus](../../../../../../solid-torus.md), removes the integer $a$, leaving the longitude. Gluing a second [solid torus](../../../../../../solid-torus.md) with meridian equal to that longitude is the standard splitting of $S^3\subset\mathbb C^2$ into the neighborhoods of its two coordinate circles. Therefore $N\cong S^3$.

By the [common nonseparating disks in a Heegaard splitting](../../../../../../common-nonseparating-disks-in-a-heegaard-splitting.md) construction and part (b), reversing the cut and caps gives

$$
\boxed{M\cong(S^1\times S^2)\mathbin\#S^3\cong S^1\times S^2.}
$$

The product metric on $S^2\times\mathbb R$ is homogeneous, and quotienting by an integer translation in the second factor gives $S^2\times S^1$. Thus $M$ carries this [Thurston geometry](../../../../../../thurston-geometry.md) and is **a [geometrizable three-manifold](../../../../../../geometrizable-three-manifold.md)**.

There is a wording qualification: if “[Heegaard genus](../../../../../../heegaard-genus.md) two” means the minimum defined in part (a), the disk data contradict it. The product splits as $S^1\times D^2$ on each hemisphere of $S^2$, giving a genus-one splitting, while genus zero gives only $S^3$, so $g_H(S^1\times S^2)=1$. The genuine construction is a genus-two splitting of a genus-one manifold; the geometrizability conclusion remains valid. The proof used the complete disk systems, the common-sphere cut-and-cap construction, and the explicitly justified genus-one meridian-intersection criterion.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

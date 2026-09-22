<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

We use [Zhang's argument](../../../../../../alternating-arms-argument-at-the-self-dual-percolation-parameter.md), obtaining the critical nonpercolation conclusion from uniqueness rather than assuming it as part of the [Harris-Kesten theorem](../../../../../../harris-kesten-theorem.md). For independent [bond percolation](../../../../../../bond-percolation-split.md) on $\mathbb Z^2$, apply part (ii) to independent [site percolation](../../../../../../site-percolation-split.md) on its [line graph](../../../../../../line-graph.md); open sites correspond to open bonds. The [line graph](../../../../../../line-graph.md) is amenable and of finite type. Therefore an infinite bond cluster, if it exists, is almost surely unique. The same holds for the [dual bond percolation](../../../../../../dual-bond-percolation.md) model.

Assume for contradiction that $\theta(1/2)>0$. The [planar dual graph](../../../../../../planar-dual-graph.md) is another [square lattice](../../../../../../square-lattice.md), and its open bonds correspond to closed primal bonds, also with parameter $1/2$. Both models then have an [infinite percolation cluster](../../../../../../infinite-percolation-cluster.md) almost surely, by part (i). As a disc $D_R$ expands, the [probability](../../../../../../probability.md) that it meets an infinite cluster tends to one, for each model. Choose $R$ avoiding all primal and dual vertices and all intersections of either graph with the four endpoints of the following arcs. Divide the boundary circle into four equal arcs $A_1,A_2,A_3,A_4$ in cyclic order. Let $L_i$ be the event of an infinite primal open ray whose last exit from $D_R$ is in $A_i$; define $L_i^*$ similarly for an infinite dual open ray. After that exit the entire ray stays outside the disc. The existence of a ray follows by finite branching in an infinite [locally finite graph](../../../../../../locally-finite-graph.md).

Each $L_i$ is increasing in the primal bond states, and their union has [probability](../../../../../../probability.md) tending to one. Four-fold rotation symmetry makes their [probabilities](../../../../../../probability.md) equal. The [FKG inequality](../../../../../../fkg-inequality.md) for their decreasing complements gives the [square-root trick for positively associated events](../../../../../../square-root-trick-for-positively-associated-events.md)

$$
\mathbb P\!\left(\bigcap_{i=1}^4 L_i^c\right)\ge\prod_{i=1}^4\mathbb P(L_i^c)=\mathbb P(L_1^c)^4.
$$

The left side tends to zero, so $\mathbb P(L_i)\to1$. Apply the same argument to the dual states to get $\mathbb P(L_i^*)\to1$. A union bound, requiring no independence between the models, now shows that for sufficiently large $R$ the alternating event

$$
L_1\cap L_2^*\cap L_3\cap L_4^*
$$

has positive [probability](../../../../../../probability.md).

The [alternating exterior-arm separation lemma](../../../../../../alternating-exterior-arm-separation-lemma.md) says that the two primal rays on this event cannot be joined by a primal open path lying outside $D_R$. Indeed, such a joining path contains a simple crosscut of the exterior between the two primal exit points. Join that crosscut to a chord inside the disc. The [Jordan curve theorem](../../../../../../jordan-curve-theorem.md) puts one of the alternating dual exit points on the bounded side. Its dual ray, which is restricted to the exterior of the disc and runs to infinity, would have to cross the open primal crosscut. A dual open bond cannot cross a primal open bond. This is impossible.

Let $F$ be the finite set of primal bonds whose drawn edges meet $D_R$, and let $E$ be the projection of the alternating-arm event onto the states outside $F$. Because $F$ is finite, this projection is a finite union of measurable events; $\mathbb P(E)>0$. Every configuration in $E$ admits an assignment on $F$ witnessing the original four arms. Now close all bonds of $F$. The infinite tails of the two primal rays beyond their first exterior vertices survive; any path joining the surviving tails would now avoid the disc. Appending their original exterior segments back to their exit points would give the forbidden exterior connection. Thus the modified configuration contains at least two [infinite percolation clusters](../../../../../../infinite-percolation-cluster.md). By independence, or the [finite-energy property of Bernoulli percolation](../../../../../../finite-energy-property-of-bernoulli-percolation.md), $\mathbb P(E\cap\{F\text{ all closed}\})=2^{-|F|}\mathbb P(E)>0$. This contradicts the uniqueness obtained from part (ii). Therefore

$$
\boxed{\theta(1/2)=0.}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The statement that limits of shape $\mathcal I$ commute with colimits of shape $\mathcal J$ means that for every $D:\mathcal I\times\mathcal J\to\mathcal C$, the canonical [commutation of limits and colimits](../../../../../commutation-of-limits-and-colimits.md) map

$$
\operatorname*{colim}_{j\in\mathcal J}\operatorname*{lim}_{i\in\mathcal I}D(i,j)
\longrightarrow
\operatorname*{lim}_{i\in\mathcal I}\operatorname*{colim}_{j\in\mathcal J}D(i,j)
$$

is an isomorphism whenever the iterated limits and colimits exist.

A [filtered category](../../../../../filtered-category.md) is a nonempty category in which every finite diagram has a cocone. Equivalently, any two objects map to a common object and any parallel pair becomes equal after postcomposition. A [weakly filtered category](../../../../../weakly-filtered-category.md) requires cocones only for finite connected diagrams; equivalently, each connected component is filtered.

Write a weakly filtered category as the disjoint union $\coprod_s\mathcal J_s$ of its filtered connected components. Its colimit is the coproduct of the filtered colimits over the $\mathcal J_s$. In sets, a connected finite limit commutes with coproducts: connectedness forces all coordinates of a compatible tuple to lie in the same coproduct summand. By the assumed theorem, the filtered colimit over each $\mathcal J_s$ commutes with every finite limit. Applying these two facts successively proves that weakly filtered colimits commute with connected finite limits in $\mathbf{Set}$.

The forgetful functor from [abelian group](../../../../../abelian-group.md) to sets creates finite limits and filtered colimits and reflects isomorphisms. The comparison map for a filtered colimit and a finite limit therefore becomes the corresponding isomorphism of sets, so filtered colimits commute with finite limits in $\mathbf{AbGp}$.

The dual claim fails because [inverse limit](../../../../../inverse-limit.md) need not preserve epimorphisms. Take the inverse systems

$$
A_n=\mathbb Z,
\qquad B_n=\mathbb Z/2^n\mathbb Z,
$$

with identity bonding maps on $A_n$, reduction maps on $B_n$, and levelwise epimorphisms $q_n:A_n\to B_n$. Then

$$
\varprojlim A_n=\mathbb Z,
\qquad
\varprojlim B_n=\mathbb Z_2,
$$

and the induced map $\mathbb Z\to\mathbb Z_2$ is not surjective. Since an epimorphism in [abelian groups](../../../../../abelian-group.md) is a finite-colimit cokernel, cofiltered limits do not commute with finite colimits in $\mathbf{AbGp}$.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

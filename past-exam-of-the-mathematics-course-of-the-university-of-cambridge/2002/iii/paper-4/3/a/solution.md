<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For each $g\ne1$, choose a [value in a lattice-ordered group](../../../../../../value-in-a-lattice-ordered-group.md) $P_g$, using [Zorn's lemma](../../../../../../zorn-s-lemma.md). Such a value is a [prime convex lattice subgroup](../../../../../../prime-convex-lattice-subgroup.md). Otherwise the last construction in Question 1(i) would give two larger [convex lattice subgroups](../../../../../../convex-lattice-subgroup.md) whose intersection is $P_g$; maximality among subgroups omitting $g$ would put $g$ in both, hence in their intersection. Thus the right coset set $\Omega_g=P_g\backslash G$ is a [totally ordered set](../../../../../../totally-ordered-set.md).

Right multiplication defines an action $\rho_g(a):P_gh\mapsto P_gha$. It is well-defined, preserves the [total order](../../../../../../total-order.md), and has inverse $\rho_g(a^{-1})$. The coset formulas from Question 1(i) show pointwise preservation of both [join](../../../../../../least-upper-bound-in-a-partially-ordered-set.md) and [meet](../../../../../../greatest-lower-bound-in-a-partially-ordered-set.md), because

$$
P_gha\vee P_ghb=P_g(ha\vee hb)=P_gh(a\vee b),
$$

and likewise for the [meet](../../../../../../greatest-lower-bound-in-a-partially-ordered-set.md).

Take the disjoint union of these chains, arranged in any fixed [order sum](../../../../../../order-sum.md) of the indices $g\ne1$. Let every $a\in G$ act on each component by $\rho_g(a)$. This gives a [lattice-ordered group homomorphism](../../../../../../lattice-ordered-group-homomorphism.md) into the [order automorphisms](../../../../../../order-automorphism.md) of one chain. It is injective: a nonidentity $a$ moves the identity coset in $\Omega_a$, since $P_aa\ne P_a$. Its image is closed under pointwise [join](../../../../../../least-upper-bound-in-a-partially-ordered-set.md) and [meet](../../../../../../greatest-lower-bound-in-a-partially-ordered-set.md), giving exactly the required [lattice-ordered permutation group](../../../../../../lattice-ordered-permutation-group.md). This is the [Holland representation theorem](../../../../../../holland-representation-theorem.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

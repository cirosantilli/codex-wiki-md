<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The law is a ferromagnetic [Ising model](../../../../../../ising-model.md) with unit couplings and no field. Its masses are strictly positive. Put $H(\sigma)=\sum_{\{x,y\}\in E}\sigma_x\sigma_y$, so $\pi(\sigma)=Z^{-1}e^{H(\sigma)}$. The order is coordinatewise with $-1<1$, which identifies the configuration space with a [Boolean lattice](../../../../../../boolean-lattice.md).

Use the permitted reduction to pairs that disagree at no more than two [graph vertices](../../../../../../vertex-graph-theory.md). If such a pair is comparable, its join and meet are the two original configurations, so the lattice inequality is equality. In the incomparable case, let the two differing [graph vertices](../../../../../../vertex-graph-theory.md) be $x,y$, with one configuration taking $(1,-1)$ there and the other $(-1,1)$. Their join takes $(1,1)$ and their meet $(-1,-1)$.

Every [edge](../../../../../../edge-of-a-graph.md) not joining $x$ to $y$ cancels in

$$
H(\sigma\vee\tau)+H(\sigma\wedge\tau)-H(\sigma)-H(\tau):
$$

a fixed [edge](../../../../../../edge-of-a-graph.md) has the same contribution throughout, while an [edge](../../../../../../edge-of-a-graph.md) from a changed [graph vertex](../../../../../../vertex-graph-theory.md) to a fixed [graph vertex](../../../../../../vertex-graph-theory.md) has the same sum of its two endpoint-spin products before and after. An [edge](../../../../../../edge-of-a-graph.md) between $x$ and $y$ contributes $1+1-(-1)-(-1)=4$. Thus the difference is nonnegative, whether or not the two changed [graph vertices](../../../../../../vertex-graph-theory.md) are adjacent. Exponentiation, with the normalizing constants cancelling, proves the [FKG lattice condition](../../../../../../fkg-lattice-condition.md) for these pairs, and hence for all pairs by the given reduction.

Equivalently one can see the full [ferromagnetic Ising lattice inequality](../../../../../../ferromagnetic-ising-lattice-inequality.md) directly. Let $U=\{x:\sigma_x=1,\tau_x=-1\}$ and $W=\{x:\sigma_x=-1,\tau_x=1\}$. Exactly the [edges](../../../../../../edge-of-a-graph.md) between $U$ and $W$ contribute, each by four. Therefore

$$
\frac{\pi(\sigma\vee\tau)\pi(\sigma\wedge\tau)}{\pi(\sigma)\pi(\tau)}
=\exp\bigl(4\,\#\{\text{edges between }U\text{ and }W\}\bigr)\ge1.
$$

The preceding part now gives

$$
\boxed{\pi(fg)\ge\pi(f)\pi(g)\quad\text{for every pair of increasing functions }f,g,}
$$

so the measure is positively associated. The sign of the coupling is essential to this argument: positive couplings favor agreement and give the nonnegative lattice difference.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

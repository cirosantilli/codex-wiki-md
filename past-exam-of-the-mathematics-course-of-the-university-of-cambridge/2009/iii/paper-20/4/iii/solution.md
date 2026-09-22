<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The geometric argument uses the [Mixed Heegaard Floer invariant](../../../../../../mixed-heegaard-floer-invariant.md) defined in Question 5(iii). First suppose $g(\Sigma)>0$; the genus-zero qualification is discussed below. Write $r=\Sigma\cdot\Sigma\ge0$. Blow up $r$ distinct points of the surface. Its proper transform $\widetilde\Sigma$ in $\widetilde M=M\#r\overline{\mathbb{CP}}^{\,2}$ has class

$$
[\widetilde\Sigma]=[\Sigma]-E_1-\cdots-E_r,\qquad\widetilde\Sigma^2=r-r=0,\qquad g(\widetilde\Sigma)=g(\Sigma).
$$

Choose the extension of the [Spin-c structure](../../../../../../spin-c-structure.md) with

$$
c_1(\widetilde{\mathfrak s})=c_1(\mathfrak s)+\sum_{j=1}^r\operatorname{PD}(E_j).
$$

Since $E_j^2=-1$, its exceptional evaluations are $-1$, so the [Blowup formula for the mixed Heegaard Floer invariant](../../../../../../blowup-formula-for-the-mixed-heegaard-floer-invariant.md) has no extra power of $U$. Thus $\Phi_{\widetilde M,\widetilde{\mathfrak s}}\ne0$, and

$$
\langle c_1(\widetilde{\mathfrak s}),[\widetilde\Sigma]\rangle=\langle c_1(\mathfrak s),[\Sigma]\rangle+r.
$$

This calculation is why the [self-intersection](../../../../../../self-intersection-number.md) appears with a plus sign.

It remains to bound the Chern pairing for a square-zero surface $S$. Its oriented [normal bundle](../../../../../../normal-bundle.md) has [Euler number](../../../../../../euler-number-of-a-vector-bundle.md) zero and is trivial, so $\partial\nu S=S\times S^1$. Choose an embedded positive-square surface $T$ disjoint from $S$, with positive direction left in its complement, and cut along $N=\partial\nu T$. To see why the choice is possible, impose orthogonality to $[S]$ in the [intersection form](../../../../../../intersection-form.md). A nonzero isotropic class uses at most one positive direction; $b_2^+\ge3$ therefore leaves at least two. Choose an integral positive-square class in that complement, represent it by a surface, and remove algebraically cancelling intersections with $S$ by tubing along $S$. This alters [genus](../../../../../../genus-of-a-surface.md) but not the class. The neighborhood of $T$ supplies one positive direction and the complement supplies another. Since its normal [Euler number](../../../../../../euler-number-of-a-vector-bundle.md) is nonzero, $H^1(\nu T)\to H^1(N)$ is onto, proving that the cut is admissible.

Put the outgoing puncture inside $\nu S$, so that the plus [Heegaard Floer cobordism map](../../../../../../heegaard-floer-cobordism-map.md) on the side containing $S$ passes through the Floer group of $\partial\nu S$. On the chain level this means splitting the [cobordism](../../../../../../cobordism.md) along that boundary and composing its handle maps; with the fixed determinant class, every intermediate generator has restriction $\mathfrak t=\widetilde{\mathfrak s}|_{S\times S^1}$. If the Chern pairing exceeded $2g(S)-2$, the given completed minus group would be zero. As in Question 3, this is the completed convention: for a non-torsion structure, ordinary infinity may retain $(1-U^N)$-torsion, whereas $1-U^N$ is invertible after completion. Such a pairing is positive for $g\ge1$, so $\mathfrak t$ is non-torsion and the completed infinity group $\mathbf{HF}^\infty(S\times S^1,\mathfrak t)$ is zero as well. The completed fundamental [long exact sequence](../../../../../../long-exact-sequence.md), whose plus group is the usual plus theory, then makes that plus group zero. The [Heegaard Floer cobordism map](../../../../../../heegaard-floer-cobordism-map.md), and consequently the [Mixed Heegaard Floer invariant](../../../../../../mixed-heegaard-floer-invariant.md), would vanish, contradicting nonvanishing. Therefore

$$
\langle c_1(\widetilde{\mathfrak s}),[\widetilde\Sigma]\rangle\le2g(\widetilde\Sigma)-2.
$$

Substituting the preceding blowup calculation proves

$$
\boxed{\langle c_1(\mathfrak s),[\Sigma]\rangle+\Sigma\cdot\Sigma\le2g(\Sigma)-2.}
$$

Reversing the orientation of the surface gives the usual absolute-value form of the [Adjunction inequality for the mixed Heegaard Floer invariant](../../../../../../adjunction-inequality-for-the-mixed-heegaard-floer-invariant.md).

**The printed assumptions omit the positive-genus qualification.** With the actual Floer groups, the asserted three-dimensional vanishing is false for $S=S^2$: the torsion structure on $S^2\times S^1$ has two nonzero minus towers, although its pairing is $0>-2$. Correspondingly, a small [sphere](../../../../../../sphere.md) embedded in a ball of a [K3 surface](../../../../../../k3-surface.md) has $[S]=0$, $S^2=0$ and Chern pairing zero, while the canonical [Mixed Heegaard Floer invariant](../../../../../../mixed-heegaard-floer-invariant.md) is nonzero; the desired inequality would read $0\le-2$. Thus the displayed proof establishes the intended positive-genus statement. If the supplied vanishing is instead taken literally as a formal additional axiom for every [genus](../../../../../../genus-of-a-surface.md), the same factorization would force the inequality even for a [sphere](../../../../../../sphere.md), but that axiom contradicts the actual $S^2\times S^1$ computation.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

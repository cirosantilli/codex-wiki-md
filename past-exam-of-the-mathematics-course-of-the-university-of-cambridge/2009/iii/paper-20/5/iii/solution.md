<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Remove two disjoint four-balls from $M$, giving $W:S^3\to S^3$. An [Admissible cut for a Heegaard Floer mixed map](../../../../../../admissible-cut-for-a-heegaard-floer-mixed-map.md) is a separating three-manifold $N$ with

$$
W=W_1\cup_N W_2,\qquad b_2^+(W_1),b_2^+(W_2)>0,\qquad\delta H^1(N;\mathbb Z)=0\subset H^2(W;\mathbb Z).
$$

The last condition is the Mayer-Vietoris connecting-map condition. It makes a [Spin-c structure](../../../../../../spin-c-structure.md) on $W$ uniquely determined by its restrictions to the two pieces, avoiding an uncontrolled sum of extensions in the composition law. Such cuts exist when $b_2^+(M)>1$: represent an integral positive-square class by an embedded surface whose tubular neighborhood carries one positive direction and whose complement retains another. One can construct an embedded representative by resolving intersections of a representative cycle; the [genus](../../../../../../genus-of-a-surface.md) may increase without changing its class or square. The nonzero normal [Euler number](../../../../../../euler-number-of-a-vector-bundle.md) makes the restriction $H^1(\nu T)\to H^1(\partial\nu T)$ surjective, so the connecting-map condition holds. Puncture on either side of the cut.

Write $\mathfrak t=\mathfrak s|_N$ and $\mathfrak s_i=\mathfrak s|_{W_i}$. Both infinity [Heegaard Floer cobordism maps](../../../../../../heegaard-floer-cobordism-map.md) vanish by positivity. Naturality with respect to the exact sequence

$$
\cdots\to HF^-(N,\mathfrak t)\xrightarrow{\iota}HF^\infty(N,\mathfrak t)\xrightarrow{\pi}HF^+(N,\mathfrak t)\xrightarrow{\delta}HF^-(N,\mathfrak t)\to\cdots
$$

gives $\operatorname{im}F^-_{W_1,\mathfrak s_1}\subset\ker\iota$ and $F^+_{W_2,\mathfrak s_2}\pi=0$. Exactness identifies $\delta$ with a degree-$-1$ isomorphism from $HF^+(N)/\operatorname{im}\pi$ onto $\ker\iota$, namely the two versions of [Reduced Heegaard Floer homology](../../../../../../reduced-heegaard-floer-homology.md). Hence the inverse on these reduced groups is defined, and one forms

$$
\boxed{F^{\mathrm{mix}}_{W,\mathfrak s}=F^+_{W_2,\mathfrak s_2}\circ\delta^{-1}\circ F^-_{W_1,\mathfrak s_1}:HF^-(S^3)\to HF^+(S^3).}
$$

This is the construction of the [Mixed Heegaard Floer invariant](../../../../../../mixed-heegaard-floer-invariant.md), rather than the zero ordinary composite.

Let $\Theta^-$ be the top minus generator, of degree $-2$, and $\Theta^+$ the bottom plus generator, of degree zero. For $\zeta\in\Lambda^*(H_1(M)/\mathrm{torsion})$, insert its degree-one [homology](../../../../../../homology-split.md) actions in the [Heegaard Floer cobordism maps](../../../../../../heegaard-floer-cobordism-map.md) and define

$$
\boxed{\Phi_{M,\mathfrak s}(U^r\otimes\zeta)=\text{coefficient of }\Theta^+\text{ in }F^{\mathrm{mix}}_{W,\mathfrak s}(U^r\Theta^-\otimes\zeta).}
$$

This is an integer up to the overall orientation sign. [cobordism](../../../../../../cobordism.md) composition and associativity show independence of the admissible cut and handle choices. Equivalently, fixing the relevant orientation data removes the overall sign ambiguity.

The grading condition can be checked explicitly. Since $\chi(W)=\chi(M)-2$ and $\sigma(W)=\sigma(M)$, the sum of the ordinary [cobordism](../../../../../../cobordism.md) shifts is $d(\mathfrak s)+1$, where $d(\mathfrak s)=(c_1(\mathfrak s)^2-2\chi(M)-3\sigma(M))/4$. The inverse connecting map contributes another $+1$. Therefore the output degree on $U^r\Theta^-\otimes\zeta$ is $d(\mathfrak s)-2r-\deg\zeta$, and the displayed invariant vanishes unless $2r+\deg\zeta=d(\mathfrak s)$.

Finally, **two positive pieces are needed**, so that both infinity maps vanish and the reduced-group factorization is available. For an admissible cut the connecting-map condition and signature additivity imply that the two positive subspaces inject as orthogonal subspaces of the closed [intersection form](../../../../../../intersection-form.md); hence $b_2^+(M)\ge2$. With only one positive direction no such admissible cut exists, and a chamber-dependent construction requires extra choices. With no positive direction, the ordinary infinity maps need not vanish at all. This explains the stated bound for the invariant defined here.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
